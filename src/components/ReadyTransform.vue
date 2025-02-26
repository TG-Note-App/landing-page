<template>
    <div class="mb-24 mt-24 relative overflow-hidden">
        <!-- Enhanced Background Effects -->
        <div class="absolute inset-0 bg-gradient-to-r from-blue-600/5 via-purple-600/5 to-blue-600/5 rounded-3xl animate-gradient-slow"></div>
        <div class="absolute -top-40 -right-40 w-96 h-96 bg-blue-500/10 rounded-full blur-3xl animate-pulse-slow"></div>
        <div class="absolute -bottom-40 -left-40 w-96 h-96 bg-purple-500/10 rounded-full blur-3xl animate-pulse-slow delay-150"></div>
        
        <!-- Content Container -->
        <div class="relative grid md:grid-cols-2 gap-12 items-center bg-gray-900/50 rounded-3xl p-12 backdrop-blur-xl border border-white/10">
          <!-- Left Column -->
          <div class="space-y-6">
            <h2 class="text-3xl font-bold">
              <span class="bg-gradient-to-r from-blue-400 to-purple-400 text-transparent bg-clip-text">
                Ready to Transform Your Notes?
              </span>
            </h2>
            <p class="text-gray-300 text-lg leading-relaxed">
              Join our growing community of organized note-takers and experience the future of Telegram note management.
            </p>
            
            <!-- Benefits List -->
            <div class="space-y-4 mt-8">
              <div class="flex items-center gap-3">
                <div class="w-8 h-8 rounded-lg bg-blue-500/20 flex items-center justify-center">
                  <i class="fas fa-check text-blue-400"></i>
                </div>
                <span class="text-gray-300">No additional app required</span>
              </div>
              <div class="flex items-center gap-3">
                <div class="w-8 h-8 rounded-lg bg-purple-500/20 flex items-center justify-center">
                  <i class="fas fa-check text-purple-400"></i>
                </div>
                <span class="text-gray-300">Start organizing in seconds</span>
              </div>
              <div class="flex items-center gap-3">
                <div class="w-8 h-8 rounded-lg bg-green-500/20 flex items-center justify-center">
                  <i class="fas fa-check text-green-400"></i>
                </div>
                <span class="text-gray-300">Free during beta</span>
              </div>
            </div>

            <!-- CTA Button -->
            <button 
              @click="scrollToForm"
              class="group relative inline-flex items-center mt-4"
            >
              <div class="absolute -inset-1 bg-gradient-to-r from-blue-500 to-purple-500 rounded-full blur opacity-75 group-hover:opacity-100 transition duration-300"></div>
              <div class="relative px-8 py-4 bg-black rounded-full leading-none flex items-center gap-3 border border-white/10 group-hover:border-white/20 transition-all duration-300">
                <span class="text-lg font-semibold text-white group-hover:text-blue-200 transition-colors">Get Started Now</span>
                <i class="fas fa-arrow-right text-white group-hover:translate-x-1 transition-transform"></i>
              </div>
            </button>
          </div>
          
          <!-- Right Column: Stats -->
          <div class="relative">
            <div class="absolute inset-0 bg-gradient-to-r from-blue-500/5 to-purple-500/5 rounded-2xl blur-xl"></div>
            <div class="relative space-y-6">
              <!-- Stats Grid -->
              <div class="grid grid-cols-2 gap-6">
                <!-- Stat 1 -->
                <div class="group p-6 bg-black/20 rounded-2xl border border-white/10 hover:border-white/20 transition-all">
                  <div class="text-3xl font-bold bg-gradient-to-r from-blue-400 to-purple-400 text-transparent bg-clip-text mb-2">
                    Instant
                  </div>
                  <p class="text-gray-400">Setup Time</p>
                </div>
                
                <!-- Stat 2 -->
                <div class="group p-6 bg-black/20 rounded-2xl border border-white/10 hover:border-white/20 transition-all">
                  <div class="text-3xl font-bold bg-gradient-to-r from-purple-400 to-pink-400 text-transparent bg-clip-text mb-2">
                    Zero
                  </div>
                  <p class="text-gray-400">Extra Apps</p>
                </div>
                
                <!-- Stat 3 -->
                <div class="group p-6 bg-black/20 rounded-2xl border border-white/10 hover:border-white/20 transition-all">
                  <div class="text-3xl font-bold bg-gradient-to-r from-green-400 to-blue-400 text-transparent bg-clip-text mb-2">
                    Free
                  </div>
                  <p class="text-gray-400">During Beta</p>
                </div>
                
                <!-- Stat 4 -->
                <div class="group p-6 bg-black/20 rounded-2xl border border-white/10 hover:border-white/20 transition-all">
                  <div class="text-3xl font-bold bg-gradient-to-r from-orange-400 to-red-400 text-transparent bg-clip-text mb-2">
                    24/7
                  </div>
                  <p class="text-gray-400">Availability</p>
                </div>
              </div>
            </div>
          </div>
        </div>
    </div>
</template>

<script setup lang="ts">
const scrollToForm = () => {
  const formElement = document.querySelector('#contact')
  if (formElement) {
    formElement.scrollIntoView({ 
      behavior: 'smooth',
      block: 'start'
    })
  }
}
</script>

<style>

</style>