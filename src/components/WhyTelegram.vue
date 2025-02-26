<template>
    <div class="mb-16 sm:mb-24 mt-16 sm:mt-24 relative px-4 sm:px-0">
        <h2 class="text-2xl sm:text-4xl font-bold text-center mb-8 sm:mb-16 bg-gradient-to-r from-blue-400 via-purple-400 to-blue-400 text-transparent bg-clip-text">
          Why Choose Telegram?
        </h2>

        <div class="grid md:grid-cols-3 gap-4 sm:gap-8">
          <!-- Feature Card 1 -->
          <div class="relative p-6 sm:p-8 bg-gray-900/40 rounded-xl sm:rounded-2xl backdrop-blur-xl border border-blue-500/10 group">
            <!-- Glow Effect -->
            <div class="absolute inset-0 rounded-xl sm:rounded-2xl bg-blue-500/5"></div>
            
            <!-- Content -->
            <div class="relative">
              <div class="w-12 sm:w-16 h-12 sm:h-16 mb-4 sm:mb-6 rounded-full bg-blue-900/30 flex items-center justify-center">
                <i class="fas fa-globe text-xl sm:text-2xl text-blue-400"></i>
              </div>
              
              <h3 class="text-lg sm:text-xl font-semibold mb-2 sm:mb-4 text-blue-400">Always Available</h3>
              <p class="text-gray-400 text-sm sm:text-base">Create and access notes instantly within your Telegram</p>
            </div>
          </div>

          <!-- Feature Card 2 -->
          <div class="relative p-6 sm:p-8 bg-gray-900/40 rounded-xl sm:rounded-2xl backdrop-blur-xl border border-purple-500/10 group">
            <!-- Glow Effect -->
            <div class="absolute inset-0 rounded-xl sm:rounded-2xl bg-purple-500/5"></div>
            
            <!-- Content -->
            <div class="relative">
              <div class="w-12 sm:w-16 h-12 sm:h-16 mb-4 sm:mb-6 rounded-full bg-purple-900/30 flex items-center justify-center">
                <i class="fas fa-shield-halved text-xl sm:text-2xl text-purple-400"></i>
              </div>
              
              <h3 class="text-lg sm:text-xl font-semibold mb-2 sm:mb-4 text-purple-400">Secure</h3>
              <p class="text-gray-400 text-sm sm:text-base">Your notes are encrypted and safely stored</p>
            </div>
          </div>

          <!-- Feature Card 3 -->
          <div class="relative p-6 sm:p-8 bg-gray-900/40 rounded-xl sm:rounded-2xl backdrop-blur-xl border border-green-500/10 group">
            <!-- Glow Effect -->
            <div class="absolute inset-0 rounded-xl sm:rounded-2xl bg-green-500/5"></div>
            
            <!-- Content -->
            <div class="relative">
              <div class="w-12 sm:w-16 h-12 sm:h-16 mb-4 sm:mb-6 rounded-full bg-green-900/30 flex items-center justify-center">
                <i class="fas fa-infinity text-xl sm:text-2xl text-green-400"></i>
              </div>
              
              <h3 class="text-lg sm:text-xl font-semibold mb-2 sm:mb-4 text-green-400">Unlimited</h3>
              <p class="text-gray-400 text-sm sm:text-base">No artificial limits on your note-taking capacity</p>
            </div>
          </div>
        </div>
      </div>
</template>

<script setup lang="ts">
</script>

<style>

</style>