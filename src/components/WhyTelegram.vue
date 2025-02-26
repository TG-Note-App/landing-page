<template>
    <div class="mb-24 mt-24 relative">
        <h2 class="text-4xl font-bold text-center mb-16 bg-gradient-to-r from-blue-400 via-purple-400 to-blue-400 text-transparent bg-clip-text">
          Why Choose Telegram?
        </h2>

        <div class="grid md:grid-cols-3 gap-8">
          <!-- Feature Card 1 -->
          <div class="relative p-8 bg-gray-900/40 rounded-2xl backdrop-blur-xl border border-blue-500/10 group">
            <!-- Glow Effect -->
            <div class="absolute inset-0 rounded-2xl bg-blue-500/5"></div>
            
            <!-- Content -->
            <div class="relative">
              <div class="w-16 h-16 mb-6 rounded-full bg-blue-900/30 flex items-center justify-center">
                <i class="fas fa-globe text-2xl text-blue-400"></i>
              </div>
              
              <h3 class="text-xl font-semibold mb-4 text-blue-400">Always Available</h3>
              <p class="text-gray-400">Create and access notes instantly within your Telegram</p>
            </div>
          </div>

          <!-- Feature Card 2 -->
          <div class="relative p-8 bg-gray-900/40 rounded-2xl backdrop-blur-xl border border-purple-500/10 group">
            <!-- Glow Effect -->
            <div class="absolute inset-0 rounded-2xl bg-purple-500/5"></div>
            
            <!-- Content -->
            <div class="relative">
              <div class="w-16 h-16 mb-6 rounded-full bg-purple-900/30 flex items-center justify-center">
                <i class="fas fa-shield-halved text-2xl text-purple-400"></i>
              </div>
              
              <h3 class="text-xl font-semibold mb-4 text-purple-400">Secure</h3>
              <p class="text-gray-400">Your notes are encrypted and safely stored</p>
            </div>
          </div>

          <!-- Feature Card 3 -->
          <div class="relative p-8 bg-gray-900/40 rounded-2xl backdrop-blur-xl border border-green-500/10 group">
            <!-- Glow Effect -->
            <div class="absolute inset-0 rounded-2xl bg-green-500/5"></div>
            
            <!-- Content -->
            <div class="relative">
              <div class="w-16 h-16 mb-6 rounded-full bg-green-900/30 flex items-center justify-center">
                <i class="fas fa-infinity text-2xl text-green-400"></i>
              </div>
              
              <h3 class="text-xl font-semibold mb-4 text-green-400">Unlimited</h3>
              <p class="text-gray-400">No artificial limits on your note-taking capacity</p>
            </div>
          </div>
        </div>
      </div>
</template>

<script>
export default {

}
</script>

<style>

</style>