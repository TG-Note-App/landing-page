<template>
  <div class="flex flex-col items-center justify-center min-h-[85vh] mb-16 relative" id="hero">
        <!-- Background Effects -->
        <div class="absolute inset-0 -z-10">
          <div class="absolute top-1/4 left-1/4 w-96 h-96 bg-blue-500/20 rounded-full blur-3xl animate-pulse-slow"></div>
          <div class="absolute bottom-1/4 right-1/4 w-96 h-96 bg-purple-500/20 rounded-full blur-3xl animate-pulse-slow delay-150"></div>
        </div>

        <!-- Main Content -->
        <div class="max-w-4xl mx-auto text-center animate-fadeIn relative z-10 px-4">
          <!-- Enhanced Title -->
          <div class="relative mb-16">
            <!-- Enhanced gradient background effect -->
            <div class="absolute -inset-6 bg-gradient-to-r from-blue-600/20 via-purple-600/20 to-blue-600/20 blur-2xl animate-pulse-slow rounded-3xl"></div>
            <div class="absolute -inset-4 bg-gradient-to-r from-purple-600/10 to-blue-600/10 blur-xl animate-pulse-slow delay-150 rounded-3xl"></div>
            
            <h1 class="relative text-5xl md:text-7xl font-bold mb-8 leading-tight">
              <!-- First line with enhanced gradient and animation -->
              <span class="inline-block w-full transform hover:scale-[1.02] transition-transform duration-500">
                <span class=" pb-2 bg-gradient-to-r from-blue-300 via-blue-400 to-purple-400 text-transparent bg-clip-text animate-gradient-slow block">
                  Telegram Mini App
                </span>
              </span>
              
              <!-- Second line with different gradient and staggered animation -->
              <span class="inline-block w-full transform hover:scale-[1.02] transition-transform duration-500 delay-100">
                <span class="bg-gradient-to-r from-purple-400 via-purple-300 to-blue-400 text-transparent bg-clip-text animate-gradient-slow delay-150 block mt-3 pb-2">
                  For Your Notes
                </span>
              </span>
            </h1>
            
            <!-- Optional subtle decorative elements -->
            <div class="absolute -right-4 top-0 w-24 h-24 bg-blue-500/5 rounded-full blur-2xl"></div>
            <div class="absolute -left-4 bottom-0 w-24 h-24 bg-purple-500/5 rounded-full blur-2xl"></div>
          </div>

          <!-- Enhanced Features Preview -->
          <div class="flex flex-wrap justify-center gap-4 mb-12">
            <div class="feature-pill group">
              <i class="fas fa-brain text-blue-400 group-hover:text-blue-300"></i>
              <span>AI-powered</span>
            </div>
            <div class="feature-pill group">
              <i class="fas fa-bolt text-purple-400 group-hover:text-purple-300"></i>
              <span>Lightning Fast</span>
            </div>
            <div class="feature-pill group">
              <i class="fas fa-shield-halved text-green-400 group-hover:text-green-300"></i>
              <span>Secure</span>
            </div>
          </div>

          <!-- Enhanced Subtitle -->
          <div class="space-y-8 mb-12">
            <p class="text-xl md:text-4xl lg:text-5xl text-gray-300 font-light leading-relaxed backdrop-blur-sm">
              <!-- Main Container with Enhanced Layout -->
              <span class="flex flex-col md:flex-row items-center justify-center gap-4 md:gap-2">
                <!-- First Part with Floating Animation -->
                <span class="inline-block transform hover:scale-[1.02] transition-all duration-500 relative group">
                  <span class="relative z-10">Transform your</span>
                  <!-- Subtle Background Glow -->
                  <div class="absolute inset-0 bg-gradient-to-r from-blue-500/5 to-purple-500/5 blur-xl opacity-0 group-hover:opacity-100 transition-all duration-700"></div>
                </span>
                
                <!-- Saved Messages Section with Enhanced Effects -->
                <span class="relative inline-flex items-center group/saved px-6 py-2">
                  <!-- Animated Gradient Background -->
                  <div class="absolute inset-0 bg-gradient-to-r from-blue-600/10 via-purple-600/10 to-blue-600/10 rounded-xl opacity-0 group-hover/saved:opacity-100 transition-all duration-500"></div>
                  
                  <!-- Main Text with Enhanced Typography -->
                  <span class="relative">
                    <span class="text-2xl font-semibold bg-gradient-to-r from-blue-300 via-purple-300 to-blue-300 bg-clip-text text-transparent animate-gradient-slow">
                      Saved Messages
                    </span>
                  </span>
                </span>

                <!-- Connecting Word with Fade Effect -->
                <span class="text-2xl inline-block transform hover:scale-[1.02] transition-all duration-500 opacity-75 group-hover:opacity-100">
                  into a
                </span>
                
                <!-- Workspace Section with Interactive Elements -->
                <span class="relative inline-flex items-center group/workspace px-6 py-2">
                  <!-- Dynamic Background -->
                  <div class="absolute inset-0 bg-gradient-to-r from-purple-600/10 via-blue-600/10 to-purple-600/10 rounded-xl opacity-0 group-hover/workspace:opacity-100 transition-all duration-500"></div>
                  
                  <!-- Main Text with Enhanced Style -->
                  <span class="relative">
                    <span class="text-2xl font-semibold bg-gradient-to-r from-purple-300 via-blue-300 to-purple-300 bg-clip-text text-transparent animate-gradient-slow">
                      Person Workspace
                    </span>
                    
                    <!-- Interactive Underline -->
                    <div class="absolute bottom-0 left-0 w-full h-0.5 bg-gradient-to-r from-purple-500/40 via-blue-500/40 to-purple-500/40 transform origin-left scale-x-0 group-hover/workspace:scale-x-100 transition-transform duration-700 ease-out"></div>
                  </span>
                </span>
              </span>
            </p>
          </div>

          <!-- Enhanced CTA Section -->
          <div class="space-y-8">
            <div class="flex flex-col sm:flex-row gap-6 justify-center items-center">
              <button 
                @click="scrollToForm"
                class="group relative inline-flex items-center scale-105 hover:scale-110 transition-all duration-300"
              >
                <!-- Reduced Glow Effects -->
                <div class="absolute -inset-1 bg-gradient-to-r from-blue-600 via-purple-600 to-blue-600 rounded-full blur-lg opacity-40 group-hover:opacity-70 transition duration-300 animate-gradient-slow"></div>
                <div class="absolute -inset-1 bg-gradient-to-r from-blue-500/30 to-purple-500/30 rounded-full blur-sm group-hover:blur-md transition-all duration-300"></div>
                
                <!-- Button Content -->
                <div class="relative px-8 py-4 bg-black rounded-full leading-none flex items-center gap-3 border border-white/20 group-hover:border-white/30 transition-all duration-300 overflow-hidden">
                  <!-- Subtle Hover Shine Effect -->
                  <div class="absolute inset-0 translate-x-[-100%] group-hover:translate-x-[100%] transition-transform duration-700 bg-gradient-to-r from-transparent via-white/5 to-transparent"></div>
                  
                  <span class="text-xl font-semibold bg-gradient-to-r from-blue-200 via-white to-purple-200 bg-clip-text text-transparent group-hover:opacity-90 transition-opacity">
                    Попробуй сейчас
                  </span>
                  <i class="fas fa-arrow-right text-lg text-white group-hover:translate-x-1 group-hover:scale-105 transition-all duration-300"></i>
                </div>
              </button>
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