<template>
  <div class="mb-16 sm:mb-24 mt-16 sm:mt-24 relative overflow-hidden px-4 sm:px-0" id="early-access">
        <!-- Enhanced Background Effects -->
        <div class="absolute inset-0 bg-gradient-to-r from-blue-600/10 via-purple-600/10 to-blue-600/10 rounded-3xl animate-gradient-slow"></div>
        <div class="absolute inset-0 bg-[url('/noise.png')] opacity-10 mix-blend-overlay"></div>
        <div class="absolute -top-20 sm:-top-40 -right-20 sm:-right-40 w-48 sm:w-96 h-48 sm:h-96 bg-blue-500/10 rounded-full blur-3xl animate-pulse-slow"></div>
        <div class="absolute -bottom-20 sm:-bottom-40 -left-20 sm:-left-40 w-48 sm:w-96 h-48 sm:h-96 bg-purple-500/10 rounded-full blur-3xl animate-pulse-slow delay-150"></div>
        
        <!-- Enhanced Content Container -->
        <div class="relative grid md:grid-cols-2 gap-8 sm:gap-12 items-center bg-gray-900/50 rounded-2xl sm:rounded-3xl p-6 sm:p-12 backdrop-blur-xl border border-white/10 hover:border-white/20 transition-all duration-500 shadow-2xl">
          <!-- Left Column -->
          <div class="relative">
            <!-- Decorative Line -->
            <div class="absolute -left-3 sm:-left-6 top-0 w-0.5 sm:w-1 h-full bg-gradient-to-b from-blue-500/50 via-purple-500/50 to-transparent rounded-full"></div>
            
            <h2 class="text-2xl sm:text-4xl font-bold mb-4 sm:mb-6 relative">
              <div class="absolute -inset-1 bg-gradient-to-r from-blue-600/20 to-purple-600/20 blur-xl animate-pulse-slow"></div>
              <span class="relative bg-gradient-to-r from-white via-blue-100 to-purple-100 bg-clip-text text-transparent">
                Be Among the First Users
              </span>
            </h2>
            
            <div class="space-y-4 sm:space-y-6 text-gray-300">
              <p class="text-base sm:text-lg leading-relaxed backdrop-blur-sm">
                We're just getting started and looking for early adopters who want to shape the future of note-taking in Telegram.
              </p>
              
              <!-- Enhanced Benefits List -->
              <div class="space-y-3 sm:space-y-4 mt-6 sm:mt-8">
                <div class="group flex items-center gap-3 sm:gap-4 p-3 sm:p-4 bg-white/5 rounded-xl border border-white/10 hover:border-white/20 hover:bg-white/10 transition-all duration-300 transform hover:translate-x-2">
                  <div class="w-10 h-10 sm:w-12 sm:h-12 rounded-xl bg-blue-500/20 flex items-center justify-center group-hover:scale-110 transition-transform">
                    <i class="fas fa-comments text-sm sm:text-base text-blue-400 group-hover:text-blue-300"></i>
                  </div>
                  <div>
                    <h3 class="font-medium text-sm sm:text-base text-white group-hover:text-blue-200 transition-colors">Direct Feedback Channel</h3>
                    <p class="text-xs sm:text-sm text-gray-400">Shape the features you want to see</p>
                  </div>
                </div>
                
                <div class="group flex items-center gap-3 sm:gap-4 p-3 sm:p-4 bg-white/5 rounded-xl border border-white/10 hover:border-white/20 hover:bg-white/10 transition-all duration-300 transform hover:translate-x-2">
                  <div class="w-10 h-10 sm:w-12 sm:h-12 rounded-xl bg-purple-500/20 flex items-center justify-center group-hover:scale-110 transition-transform">
                    <i class="fas fa-gem text-sm sm:text-base text-purple-400 group-hover:text-purple-300"></i>
                  </div>
                  <div>
                    <h3 class="font-medium text-sm sm:text-base text-white group-hover:text-purple-200 transition-colors">Early Access Benefits</h3>
                    <p class="text-xs sm:text-sm text-gray-400">Get features before they're widely available</p>
                  </div>
                </div>
              </div>
            </div>
            
            <!-- Enhanced CTA Button -->
            <div class="mt-8 sm:mt-12">
              <button 
                @click="scrollToForm"
                class="group relative inline-flex items-center"
              >
                <div class="absolute -inset-1 bg-gradient-to-r from-blue-500 to-purple-500 rounded-full blur opacity-75 group-hover:opacity-100 transition duration-300 animate-pulse-slow"></div>
                <div class="relative px-6 sm:px-8 py-3 sm:py-4 bg-black rounded-full leading-none flex items-center gap-2 sm:gap-3 border border-white/10 group-hover:border-white/20 transition-all duration-300">
                  <span class="text-base sm:text-lg font-semibold text-white group-hover:text-blue-200 transition-colors">Get the App</span>
                  <i class="fas fa-arrow-right text-sm sm:text-base text-white group-hover:translate-x-1 transition-transform"></i>
                </div>
              </button>
            </div>
          </div>
          
          <!-- Right Column -->
          <div class="relative hidden md:block">
            <!-- Enhanced Feature Preview Card -->
            <div class="group bg-gradient-to-br from-white/10 to-white/5 rounded-xl sm:rounded-2xl p-6 sm:p-8 backdrop-blur-xl border border-white/10 hover:border-white/20 transition-all duration-500 transform hover:scale-[1.02]">
              <div class="absolute inset-0 bg-gradient-to-r from-transparent via-white/5 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-500"></div>
              
              <h3 class="text-xl sm:text-2xl font-semibold text-white mb-6 sm:mb-8 bg-gradient-to-r from-blue-400 to-purple-400 bg-clip-text text-transparent">
                Coming Soon Features
              </h3>
              
              <div class="space-y-4 sm:space-y-6">
                <div class="group/item flex items-center gap-3 sm:gap-4 p-2 sm:p-3 rounded-xl hover:bg-white/5 transition-colors">
                  <div class="w-8 h-8 sm:w-10 sm:h-10 rounded-lg bg-green-500/20 flex items-center justify-center group-hover/item:scale-110 transition-transform">
                    <i class="fas fa-brain text-sm sm:text-base text-green-400 group-hover/item:text-green-300"></i>
                  </div>
                  <span class="text-sm sm:text-base text-gray-300 group-hover/item:text-white transition-colors">AI-powered Note Organization</span>
                </div>
                
                <div class="group/item flex items-center gap-3 sm:gap-4 p-2 sm:p-3 rounded-xl hover:bg-white/5 transition-colors">
                  <div class="w-8 h-8 sm:w-10 sm:h-10 rounded-lg bg-blue-500/20 flex items-center justify-center group-hover/item:scale-110 transition-transform">
                    <i class="fas fa-tags text-sm sm:text-base text-blue-400 group-hover/item:text-blue-300"></i>
                  </div>
                  <span class="text-sm sm:text-base text-gray-300 group-hover/item:text-white transition-colors">Smart Tagging System</span>
                </div>
                
                <div class="group/item flex items-center gap-3 sm:gap-4 p-2 sm:p-3 rounded-xl hover:bg-white/5 transition-colors">
                  <div class="w-8 h-8 sm:w-10 sm:h-10 rounded-lg bg-orange-500/20 flex items-center justify-center group-hover/item:scale-110 transition-transform">
                    <i class="fas fa-wand-magic-sparkles text-sm sm:text-base text-orange-400 group-hover/item:text-orange-300"></i>
                  </div>
                  <span class="text-sm sm:text-base text-gray-300 group-hover/item:text-white transition-colors">Customizable Templates</span>
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