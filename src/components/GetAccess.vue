<template>
    <div class="relative mb-16 sm:mb-24 px-4 sm:px-0" id="contact">
        <!-- Enhanced Background Effects -->
        <div class="absolute inset-0 bg-gradient-to-r from-blue-600/10 via-purple-600/10 to-blue-600/10 rounded-2xl sm:rounded-3xl"></div>
        <div class="absolute inset-0 bg-[url('/noise.png')] opacity-10 mix-blend-overlay"></div>
        
        <!-- Content Container -->
        <div class="relative bg-gray-900/50 rounded-2xl sm:rounded-3xl p-6 sm:p-12 backdrop-blur-xl border border-white/10">
            <div class="max-w-2xl mx-auto text-center mb-8 sm:mb-12">
            <h2 class="text-2xl sm:text-4xl font-bold mb-4 sm:mb-6">
                <span class="bg-gradient-to-r from-blue-400 via-purple-400 to-blue-400 text-transparent bg-clip-text">
                Get Early Access
                </span>
            </h2>
            <p class="text-base sm:text-lg text-gray-300 mb-6 sm:mb-8">
                Join our beta program and be among the first to experience the future of note-taking in Telegram.
            </p>
            </div>

            <!-- Contact Form -->
            <form @submit="handleSubmit" class="max-w-lg mx-auto space-y-4 sm:space-y-6">
            <div class="space-y-3 sm:space-y-4">
                <div class="relative group">
                <input 
                    v-model="email"
                    type="email" 
                    placeholder="Your email address"
                    class="w-full px-4 sm:px-6 py-3 sm:py-4 bg-black/50 rounded-xl border border-white/10 text-white text-sm sm:text-base placeholder:text-gray-500 focus:outline-none focus:border-blue-500/50 transition-all"
                    :disabled="isSubmitting"
                    required
                />
                </div>
                
                <!-- Form Message -->
                <div v-if="formMessage" 
                :class="[
                    'text-xs sm:text-sm px-3 sm:px-4 py-2 rounded-lg transition-all',
                    formMessageType === 'success' ? 'bg-green-500/20 text-green-400' : 'bg-red-500/20 text-red-400'
                ]"
                >
                {{ formMessage }}
                </div>
            </div>

            <button 
                type="submit"
                class="group relative w-full inline-flex items-center justify-center"
                :disabled="isSubmitting"
            >
                <div class="absolute -inset-0.5 bg-gradient-to-r from-blue-500 to-purple-500 rounded-full blur opacity-75 group-hover:opacity-100 transition duration-300"></div>
                <div class="relative w-full px-6 sm:px-8 py-3 sm:py-4 bg-black rounded-full leading-none flex items-center justify-center gap-2 sm:gap-3 border border-white/10 group-hover:border-white/20 transition-all duration-300">
                <span v-if="isSubmitting" class="text-base sm:text-lg font-semibold text-white">
                    <i class="fas fa-spinner fa-spin mr-2"></i>Submitting...
                </span>
                <span v-else class="text-base sm:text-lg font-semibold text-white group-hover:text-blue-200 transition-colors">
                    Enjoy the App
                    <i class="fas fa-arrow-right ml-2 group-hover:translate-x-1 transition-transform"></i>
                </span>
                </div>
            </button>
            </form>
        </div>
    </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

// Form state
const email = ref('')
const isSubmitting = ref(false)
const formMessage = ref('')
const formMessageType = ref<'success' | 'error' | null>(null)


const handleSubmit = async (e: Event) => {
  e.preventDefault()

  // Early validation to avoid unnecessary processing
  if (!email.value.trim()) {
    formMessage.value = 'Please enter an email address'
    formMessageType.value = 'error'
    return
  }

  // Simple regex check instead of full validation function
  if (!email.value.match(/^[^\s@]+@[^\s@]+\.[^\s@]+$/)) {
    formMessage.value = 'Please enter a valid email address'
    formMessageType.value = 'error'
    return
  }

  try {
    isSubmitting.value = true
    formMessage.value = '' // Clear previous messages

    // Create request data once
    const data = JSON.stringify({
      email: email.value,
      timestamp: new Date().toISOString()
    })

    // Use Promise.race to implement a timeout
    const timeoutPromise = new Promise((_, reject) => 
      setTimeout(() => reject(new Error('Request timeout')), 5000)
    )

    // Replace the direct URL with environment variable
    const fetchPromise = fetch(import.meta.env.VITE_GOOGLE_SCRIPT_URL, {
      method: 'POST',
      mode: 'no-cors',
      headers: {
        'Content-Type': 'application/json',
      },
      body: data
    })

    await Promise.race([fetchPromise, timeoutPromise])
    
    // Success handling
    email.value = '' // Clear form
    formMessage.value = 'Thank you for joining! We will be in touch soon.'
    formMessageType.value = 'success'

  } catch (error) {
    // Error handling
    console.error('Submission error:', error)
    formMessage.value = error instanceof Error && error.message === 'Request timeout' 
      ? 'Request timed out. Please try again.'
      : 'Something went wrong. Please try again later.'
    formMessageType.value = 'error'
  } finally {
    isSubmitting.value = false
  }
}
</script>

<style>

</style>