<template>
    <footer class="border-t border-white/10 pt-12 pb-8" id="footer">
        <div class="max-w-4xl mx-auto px-4 sm:px-6">
          <!-- Main Footer Content -->
          <div class="grid md:grid-cols-3 gap-8 mb-8">
            <!-- Brand Column -->
            <div>
              <h3 class="text-xl font-bold mb-4 bg-gradient-to-r from-blue-400 to-purple-400 text-transparent bg-clip-text">
                TG Notes
              </h3>
              <p class="text-gray-400 text-sm leading-relaxed">
                Transform your messages into organized notes.
              </p>
            </div>

            <!-- Quick Links -->
            <div class="flex gap-12">
              <div>
                <h4 class="text-sm font-semibold text-white mb-3">Product</h4>
                <ul class="space-y-2">
                  <li>
                    <a href="#features-overview" class="text-sm text-gray-400 hover:text-white transition-colors">Features</a>
                  </li>
                  <li>
                    <a href="#early-access" class="text-sm text-gray-400 hover:text-white transition-colors">Beta Access</a>
                  </li>
                  <li>
                    <a href="#comparison" class="text-sm text-gray-400 hover:text-white transition-colors">Why Choose Us</a>
                  </li>
                </ul>
              </div>
            </div>

            <!-- Social Links -->
            <div class="flex justify-end items-start space-x-6">
              <!-- Telegram Link -->
              <a href="https://t.me/greenblat" 
                 class="group relative"
                 target="_blank"
                 rel="noopener noreferrer"
              >
                <div class="absolute -inset-2 bg-gradient-to-r from-blue-600/20 to-blue-400/20 rounded-lg blur-sm opacity-0 group-hover:opacity-100 transition-all duration-300"></div>
                <div class="relative w-10 h-10 rounded-lg bg-gradient-to-br from-blue-500/10 to-blue-600/10 flex items-center justify-center border border-blue-500/20 group-hover:border-blue-400/40 group-hover:bg-blue-500/20 transition-all duration-300">
                  <i class="fab fa-telegram text-xl text-blue-400 group-hover:text-blue-300 transform group-hover:scale-110 group-hover:-translate-y-0.5 transition-all duration-300"></i>
                </div>
                <span class="absolute -bottom-6 left-1/2 -translate-x-1/2 text-xs text-blue-400/80 opacity-0 group-hover:opacity-100 transition-all duration-300">Telegram</span>
              </a>

              <!-- GitHub Link -->
              <a href="https://github.com/greenblat17" 
                 class="group relative"
                 target="_blank"
                 rel="noopener noreferrer"
              >
                <div class="absolute -inset-2 bg-gradient-to-r from-purple-600/20 to-purple-400/20 rounded-lg blur-sm opacity-0 group-hover:opacity-100 transition-all duration-300"></div>
                <div class="relative w-10 h-10 rounded-lg bg-gradient-to-br from-purple-500/10 to-purple-600/10 flex items-center justify-center border border-purple-500/20 group-hover:border-purple-400/40 group-hover:bg-purple-500/20 transition-all duration-300">
                  <i class="fab fa-github text-xl text-purple-400 group-hover:text-purple-300 transform group-hover:scale-110 group-hover:-translate-y-0.5 transition-all duration-300"></i>
                </div>
                <span class="absolute -bottom-6 left-1/2 -translate-x-1/2 text-xs text-purple-400/80 opacity-0 group-hover:opacity-100 transition-all duration-300">GitHub</span>
              </a>
            </div>
          </div>

          <!-- Bottom Bar -->
          <div class="flex flex-col md:flex-row justify-between items-center gap-4 pt-8 border-t border-white/10">
            <div class="text-xs text-gray-400">
              © 2024 TG Notes. All rights reserved.
            </div>
            <div class="flex gap-4 text-xs">
              <a href="#" class="text-gray-400 hover:text-white transition-colors">Privacy</a>
              <a href="#" class="text-gray-400 hover:text-white transition-colors">Terms</a>
            </div>
          </div>
        </div>
    </footer>
</template>

<script setup lang="ts">
</script>

<style>

</style>