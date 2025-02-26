<template>
  <div class="min-h-screen bg-fixed bg-gradient-to-br from-gray-900 to-black text-white overflow-x-hidden">
    <div class="fixed inset-0 bg-gradient-to-br from-gray-900 to-black -z-50"></div>
    
    <div class="max-w-4xl mx-auto px-4 sm:px-8 py-16">
      <Hero />
      <Feature />
      <FirstUser />
      <div class="grid md:grid-cols-2 gap-20 items-center">
        <Text title="Transform Your Telegram Experience" description="Turn your cluttered Saved Messages into a powerful, organized workspace. Access everything you need instantly, without the endless scrolling." :items="[
          { icon: 'fas fa-share-nodes', iconColor: 'blue', text: 'Resend messages from any chats' },
          { icon: 'fas fa-bookmark', iconColor: 'purple', text: 'Save messages to your notes' },
          { icon: 'fas fa-bolt', iconColor: 'green', text: 'Quick access to your notes' }
        ]" />
        
        <!-- Visual: Modern Telegram Interface -->
        <Phone>
          <!-- Chat Header -->
          <div class="px-5 py-4 flex items-center gap-3 border-b border-white/5">
            <div class="w-10 h-10 rounded-full bg-blue-500 flex items-center justify-center">
              <i class="fas fa-bookmark text-white text-lg"></i>
            </div>
            <div>
              <h4 class="text-white font-medium">Saved Messages</h4>
              <p class="text-xs text-white/40">last seen recently</p>
            </div>
          </div>

          <div class="p-4 space-y-3">
            <!-- Message 1 -->
            <div class="flex justify-end">
              <div class="bg-[#2b5278] rounded-2xl rounded-tr-sm px-4 py-2 max-w-[85%]">
                <div class="flex items-center gap-2 mb-1">
                  <i class="fas fa-file-alt text-white/60 text-sm"></i>
                  <span class="text-white/80 text-sm font-medium">Project Update</span>
                </div>
                <p class="text-white text-sm leading-relaxed">Latest changes have been committed 🚀</p>
                <p class="text-[10px] text-white/40 text-right mt-1">12:30</p>
              </div>
            </div>

            <!-- Message 2 -->
            <div class="flex justify-end">
              <div class="bg-[#2b5278] rounded-2xl rounded-tr-sm px-4 py-2 max-w-[85%]">
                <div class="flex items-center gap-2 mb-1">
                  <i class="fas fa-link text-white/60 text-sm"></i>
                  <span class="text-white/80 text-sm font-medium">GitHub Link</span>
                </div>
                <p class="text-white text-sm leading-relaxed">github.com/user/project</p>
                <p class="text-[10px] text-white/40 text-right mt-1">12:31</p>
              </div>
            </div>

            <div class="flex justify-end">
              <div class="bg-[#2b5278] rounded-2xl rounded-tr-sm px-4 py-2 max-w-[85%]">
                <div class="flex items-center gap-2 mb-1">
                  <i class="fas fa-code text-white/60 text-sm"></i>
                  <span class="text-white/80 text-sm font-medium">Code Snippet</span>
                </div>
                <div class="mt-2 rounded-lg bg-black/20 p-2 font-mono">
                  <code class="text-xs text-green-400">npm install && npm run dev</code>
                </div>
                <p class="text-[10px] text-white/40 text-right mt-1">12:34</p>
              </div>
            </div>

            <!-- Forward Animation -->
            <div class="flex justify-center py-8">
              <div class="relative">
                <div class="absolute inset-0 bg-blue-500/20 rounded-full blur-xl animate-pulse"></div>
                <div class="relative w-12 h-12 rounded-full bg-gradient-to-r from-blue-500 to-purple-500 flex items-center justify-center animate-bounce-subtle">
                  <i class="fas fa-arrow-down text-white"></i>
                </div>
              </div>
            </div>
          </div>
        </Phone>    
      </div>

      <div class="grid md:grid-cols-2 gap-20 items-center mt-24">
          
          <!-- Visual: Modern Telegram Interface -->
        <Phone>
          <div class="h-full w-full relative">
            <div class="px-5 py-4 flex items-center justify-between border-b border-white/10 backdrop-blur-sm bg-black/20">
              <div>
                <h4 class="text-white text-xl font-medium">Notes</h4>
                <p class="text-xs text-white/40">Welcome back, Alex</p>
              </div>
              <button class="relative group">
                <div class="absolute -inset-1 bg-gradient-to-r from-blue-500 to-purple-500 rounded-full blur opacity-60 group-hover:opacity-100 transition duration-200"></div>
                <div class="relative w-10 h-10 rounded-full bg-black flex items-center justify-center border border-white/10 group-hover:border-white/20">
                  <i class="fas fa-plus text-transparent bg-gradient-to-r from-blue-400 to-purple-400 bg-clip-text group-hover:scale-110 transition-all"></i>
                </div>
              </button>
            </div>

            <!-- Search Bar -->
            <div class="p-4">
              <div class="relative group">
                <div class="absolute inset-0 bg-gradient-to-r from-blue-500/20 to-purple-500/20 rounded-xl blur-sm opacity-0 group-hover:opacity-100 transition duration-300"></div>
                <div class="relative flex items-center gap-3 bg-white/5 rounded-xl px-4 py-2.5 border border-white/10 group-hover:border-white/20 transition-all duration-300">
                  <i class="fas fa-magnifying-glass text-white/40 group-hover:text-white/60 transition-colors"></i>
                  <input 
                    type="text" 
                    placeholder="Search notes..." 
                    class="bg-transparent w-full text-white placeholder-white/40 focus:placeholder-white/60 outline-none text-sm"
                  />

                </div>
              </div>
            </div>

            <!-- Notes List -->
            <div class="px-4 space-y-3 relative">
              <!-- Floating Action Button -->
              <button 
                @click="scrollToTop"
                class="fixed bottom-6 right-6 group opacity-0 transition-all duration-300"
                :class="{ 'opacity-100': showScrollToTop }"
              >
                <div class="absolute -inset-2 bg-gradient-to-r from-blue-500 to-purple-500 rounded-full blur opacity-75 group-hover:opacity-100 animate-pulse-slow"></div>
                <div class="relative p-4 bg-black rounded-full border border-white/10 group-hover:border-white/20 transition-all">
                  <i class="fas fa-arrow-up text-white group-hover:-translate-y-1 transition-all duration-300"></i>
                </div>
              </button>

              <!-- Note Items -->
              <div class="space-y-3">
                <!-- Note 1 -->
                <div class="group relative">
                  <div class="absolute inset-0 bg-gradient-to-r from-blue-500/20 via-purple-500/20 to-blue-500/20 rounded-xl blur-sm opacity-0 group-hover:opacity-100 transition duration-300"></div>
                  <div class="relative p-4 bg-white/5 rounded-xl hover:bg-white/10 transition-all border border-white/10 group-hover:border-white/20">
                    <div class="flex items-start gap-4">
                      <div class="shrink-0">
                        <div class="w-10 h-10 rounded-lg bg-gradient-to-br from-blue-500/20 to-purple-500/20 flex items-center justify-center group-hover:scale-110 transition-transform">
                          <i class="fas fa-code text-blue-400 group-hover:text-blue-300"></i>
                        </div>
                      </div>
                      <div class="flex-1 min-w-0">
                        <div class="flex items-center justify-between mb-1">
                          <h4 class="text-white font-medium truncate">API Integration</h4>
                          <span class="text-xs text-white/40">2m ago</span>
                        </div>
                        <p class="text-sm text-gray-400 line-clamp-2 mb-2">Implementation steps...</p>
                        <div class="flex items-center gap-2">
                          <span class="px-2 py-1 text-xs rounded-full bg-blue-500/10 text-blue-400 border border-blue-500/20">#coding</span>
                          <span class="px-2 py-1 text-xs rounded-full bg-purple-500/10 text-purple-400 border border-purple-500/20">#api</span>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>

                <!-- Note 2 -->
                <div class="group relative">
                  <div class="absolute inset-0 bg-gradient-to-r from-green-500/20 via-emerald-500/20 to-green-500/20 rounded-xl blur-sm opacity-0 group-hover:opacity-100 transition duration-300"></div>
                  <div class="relative p-4 bg-white/5 rounded-xl hover:bg-white/10 transition-all border border-white/10 group-hover:border-white/20">
                    <div class="flex items-start gap-4">
                      <div class="shrink-0">
                        <div class="w-10 h-10 rounded-lg bg-gradient-to-br from-green-500/20 to-emerald-500/20 flex items-center justify-center group-hover:scale-110 transition-transform">
                          <i class="fas fa-list-check text-green-400 group-hover:text-green-300"></i>
                        </div>
                      </div>
                      <div class="flex-1 min-w-0">
                        <div class="flex items-center justify-between mb-1">
                          <h4 class="text-white font-medium truncate">Project Roadmap</h4>
                          <span class="text-xs text-white/40">1h ago</span>
                        </div>
                        <p class="text-sm text-gray-400 line-clamp-2 mb-2">Q1 Goals: 1. Launch beta...</p>
                        <div class="flex items-center gap-2">
                          <span class="px-2 py-1 text-xs rounded-full bg-green-500/10 text-green-400 border border-green-500/20">#planning</span>
                          <span class="px-2 py-1 text-xs rounded-full bg-emerald-500/10 text-emerald-400 border border-emerald-500/20">#goals</span>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>

                <!-- Note 3 -->
                <div class="group relative">
                  <div class="absolute inset-0 bg-gradient-to-r from-orange-500/20 via-yellow-500/20 to-orange-500/20 rounded-xl blur-sm opacity-0 group-hover:opacity-100 transition duration-300"></div>
                  <div class="relative p-4 bg-white/5 rounded-xl hover:bg-white/10 transition-all border border-white/10 group-hover:border-white/20">
                    <div class="flex items-start gap-4">
                      <div class="shrink-0">
                        <div class="w-10 h-10 rounded-lg bg-gradient-to-br from-orange-500/20 to-yellow-500/20 flex items-center justify-center group-hover:scale-110 transition-transform">
                          <i class="fas fa-lightbulb text-orange-400 group-hover:text-orange-300"></i>
                        </div>
                      </div>
                      <div class="flex-1 min-w-0">
                        <div class="flex items-center justify-between">
                          <h4 class="text-white text-sm font-medium truncate">Feature Ideas</h4>
                          <span class="text-xs text-white/40">3h ago</span>
                        </div>
                        <p class="text-xs text-gray-400 line-clamp-1 my-1">New UI improvements for v2...</p>
                        <div class="flex items-center gap-2">
                          <span class="px-1.5 py-0.5 text-xs rounded-full bg-orange-500/10 text-orange-400 border border-orange-500/20">#ideas</span>
                          <span class="px-1.5 py-0.5 text-xs rounded-full bg-yellow-500/10 text-yellow-400 border border-yellow-500/20">#ui</span>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </Phone>
         

          <Text title="Organized Notes" description="Keep your notes neatly organized with folders, tags, and smart categorization." :items="[
            { icon: 'fas fa-folder-tree', iconColor: 'blue', text: 'Create custom folders' },
            { icon: 'fas fa-tags', iconColor: 'purple', text: 'Tag and categorize notes' },
            { icon: 'fas fa-magnifying-glass', iconColor: 'green', text: 'Smart search and filters' }
          ]" />
        </div>

        <div class="grid md:grid-cols-2 gap-20 items-center mt-24">

          <Text title="Editing Notes and Store Files" description="Powerful editing tools and file management to keep your content organized and accessible." :items="[
            { icon: 'fas fa-pen-to-square', iconColor: 'blue', text: 'Rich text editor with formatting' },
            { icon: 'fas fa-folder-open', iconColor: 'purple', text: 'Store and organize any file type' },
            { icon: 'fas fa-cloud', iconColor: 'green', text: 'Cloud sync and backup' }
          ]" />
          
          <!-- Visual: Modern Telegram Interface -->
          <Phone>
            <div class="px-5 py-4 flex items-center gap-4 border-b border-white/5 backdrop-blur-sm bg-black/20">

              <!-- Back Button -->
              <button class="group relative p-0.5">
                <div class="absolute inset-0 bg-gradient-to-r from-blue-500/20 to-purple-500/20 rounded-lg opacity-0 group-hover:opacity-100 transition-all duration-300"></div>
                <div class="relative w-8 h-8 rounded-lg bg-white/5 flex items-center justify-center group-hover:bg-white/10 transition-all duration-300">
                  <i class="fas fa-arrow-left text-white/60 group-hover:text-white group-hover:-translate-x-0.5 transition-all duration-300"></i>
                </div>
              </button>

              <!-- Title and Metadata -->
              <div class="flex-1 min-w-0 ml-2">
                <div class="items-center">
                  <h4 class="text-white font-medium truncate">API Integration</h4>
                  <div class="flex items-center gap-1.5">
                    <i class="fas fa-folder text-xs text-blue-400"></i>
                    <span class="text-xs text-blue-400">Development</span>
                  </div>
                </div>
              </div>

              <!-- Action Buttons -->
              <div class="flex items-center gap-2">
                <button class="group relative p-0.5">
                  <div class="absolute inset-0 bg-gradient-to-r from-blue-500/20 to-purple-500/20 rounded-lg opacity-0 group-hover:opacity-100 transition-all duration-300"></div>
                  <div class="relative w-8 h-8 rounded-lg bg-white/5 flex items-center justify-center group-hover:bg-white/10 transition-all duration-300">
                    <i class="fas fa-ellipsis-vertical text-white/60 group-hover:text-white group-hover:scale-110 transition-all duration-300"></i>
                  </div>
                </button>
              </div>
            </div>

          <!-- Note Content -->
          <div class="p-5 space-y-6">
              <!-- Tags -->
              <div class="flex items-center gap-2">
                <span class="px-2 py-1 text-xs rounded-full bg-blue-500/10 text-blue-400 border border-blue-500/20">
                  #coding
                </span>
                <span class="px-2 py-1 text-xs rounded-full bg-purple-500/10 text-purple-400 border border-purple-500/20">
                  #api
                </span>
              </div>

              <!-- Note Content -->
              <div class="space-y-4">
                <h1 class="text-xl font-semibold text-white">
                  API Integration Steps
                </h1>
                
                <div class="space-y-3 text-gray-300">
                  <p class="leading-relaxed">
                    Key steps for implementing the new API integration:
                  </p>
                  
                  <!-- Checklist -->
                  <div class="space-y-2">
                    <!-- Completed Task -->
                    <div class="flex items-center gap-3 p-2 bg-white/5 rounded-lg">
                      <div class="w-5 h-5 rounded bg-green-500/20 border border-green-500/30 flex items-center justify-center">
                        <i class="fas fa-check text-xs text-green-400"></i>
                      </div>
                      <span class="text-sm">Set up authentication endpoints</span>
                    </div>
                    
                    <!-- Pending Tasks -->
                    <div class="flex items-center gap-3 p-2 bg-white/5 rounded-lg">
                      <div class="w-5 h-5 rounded bg-white/10 border border-white/20 flex items-center justify-center">
                      </div>
                      <span class="text-sm">Implement data validation</span>
                    </div>
                    
                    <div class="flex items-center gap-3 p-2 bg-white/5 rounded-lg">
                      <div class="w-5 h-5 rounded bg-white/10 border border-white/20 flex items-center justify-center">
                      </div>
                      <span class="text-sm">Add error handling</span>
                    </div>
                  </div>
                </div>
              </div>
            </div>  
          </Phone> 
        </div>
      <OnePlace />
      <WhyTelegram />
      <ReadyTransform />
      <Comparison />
      <GetAccess />
      <Footer />
    </div>
  </div>
</template>

<script setup lang="ts">
import Hero from './components/Hero.vue'
import Feature from './components/Feature.vue'
import FirstUser from './components/FirstUser.vue'
import Phone from './components/Phone.vue'
import OnePlace from './components/OnePlace.vue'
import Text from './components/Text.vue'
import WhyTelegram from './components/WhyTelegram.vue'
import Footer from './components/Footer.vue'
import GetAccess from './components/GetAccess.vue'
import Comparison from './components/Comparison.vue'
import ReadyTransform from './components/ReadyTransform.vue'
import { ref, onMounted, onUnmounted } from 'vue'

let scrollTimeout: number | null = null


onMounted(() => {
  window.addEventListener('scroll', handleScroll, { passive: true })
})

const submitTimeout = ref<number | null>(null)

onUnmounted(() => {
  if (scrollTimeout) {
    window.cancelAnimationFrame(scrollTimeout)
  }
  window.removeEventListener('scroll', handleScroll)
  if (submitTimeout.value) {
    clearTimeout(submitTimeout.value)
  }
})

// Add these new refs and functions
const showScrollToTop = ref(false)

// Modify the existing handleScroll function
const handleScroll = () => {
  if (scrollTimeout) {
    window.cancelAnimationFrame(scrollTimeout)
  }

  scrollTimeout = window.requestAnimationFrame(() => {
    showScrollToTop.value = window.scrollY > 500
  })
}

// Add this new function
const scrollToTop = () => {
  window.scrollTo({
    top: 0,
    behavior: 'smooth'
  })
}
</script>

<style>
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.animate-fadeIn {
  animation: fadeIn 0.8s ease-out forwards;
  will-change: transform, opacity;
}

@keyframes pulse {
  0%, 100% {
    opacity: 1;
  }
  50% {
    opacity: .7;
  }
}

.animate-pulse {
  animation: pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
}

.shadow-lg {
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
}

.shadow-xl {
  box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1), 0 10px 10px -5px rgba(0, 0, 0, 0.04);
}

/* Floating button hover effect */
.group:hover i {
  transform: translateY(-2px);
}

.group i {
  transition: transform 0.2s ease-in-out;
}

@keyframes float {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(-10px);
  }
}

.animate-float {
  animation: float 6s ease-in-out infinite;
  will-change: transform;
  transform: translateZ(0);
}

.shadow-inner-light {
  box-shadow: inset 0 0 1px rgba(255, 255, 255, 0.1);
}

.shadow-inner-subtle {
  box-shadow: inset 0 2px 4px rgba(0, 0, 0, 0.1);
}

.text-shadow-sm {
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.2);
}

@keyframes pulse-slow {
  0%, 100% {
    opacity: 0.4;
  }
  50% {
    opacity: 0.7;
  }
}

.animate-pulse-slow {
  animation: pulse-slow 4s cubic-bezier(0.4, 0, 0.6, 1) infinite;
}

@keyframes gradient {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

.animate-gradient {
  background-size: 200% 200%;
  animation: gradient 8s ease infinite;
  will-change: background-position;
  transform: translateZ(0);
}

.bg-fixed {
  background-attachment: fixed;
}

.overflow-x-hidden {
  overflow-x: hidden;
}

/* Добавляем новые стили для выделения */
.highlight-text {
  background: linear-gradient(120deg, rgba(96, 165, 250, 0.2) 0%, rgba(168, 85, 247, 0.2) 100%);
  padding: 0.5rem 1rem;
  border-radius: 0.5rem;
  border: 1px solid rgba(255, 255, 255, 0.1);
}

.highlight-span {
  background: linear-gradient(120deg, #60a5fa 0%, #a855f7 100%);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: 600;
}

@keyframes gradient-slow {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

.animate-gradient-slow {
  background-size: 200% 200%;
  animation: gradient-slow 8s ease infinite;
}

.delay-150 {
  animation-delay: 150ms;
}

@keyframes bounce-subtle {
  0%, 100% { transform: translateY(0); }
  50% { transform: translateY(-8px); }
}

.animate-bounce-subtle {
  animation: bounce-subtle 2s ease-in-out infinite;
}

.feature-pill {
  @apply flex items-center gap-2 px-6 py-3 bg-white/5 rounded-full backdrop-blur-sm
         border border-white/10 hover:border-white/20 hover:bg-white/10 
         transition-all duration-300 cursor-default;
}

.feature-pill i {
  @apply text-lg transition-all duration-300;
}

.feature-pill span {
  @apply text-gray-300 font-medium;
}

.animate-bounce-slow {
  animation: bounce 2s infinite;
}

@keyframes bounce {
  0%, 100% {
    transform: translateY(0);
  }
  50% {
    transform: translateY(10px);
  }
}

.feature-card {
  @apply flex items-start gap-6 p-6 bg-white/5 rounded-2xl 
         hover:bg-white/10 transition-all duration-300
         border border-white/5 hover:border-white/10;
}

.preview-card {
  @apply flex items-center gap-4 p-4 bg-white/5 rounded-xl
         hover:bg-white/10 transition-all duration-300
         border border-white/5 hover:border-white/10;
}

/* Add these new styles */
.form-message-enter-active,
.form-message-leave-active {
  transition: all 0.3s ease;
}

.form-message-enter-from,
.form-message-leave-to {
  opacity: 0;
  transform: translateY(-10px);
}

/* Add these new animations to your existing styles */
@keyframes gradient-flow {
  0% { background-position: 0% 50%; }
  50% { background-position: 100% 50%; }
  100% { background-position: 0% 50%; }
}

.animate-gradient-slow {
  background-size: 200% auto;
  animation: gradient-flow 4s ease infinite;
}

@keyframes ping {
  75%, 100% {
    transform: scale(2);
    opacity: 0;
  }
}

.animate-ping {
  animation: ping 2s cubic-bezier(0, 0, 0.2, 1) infinite;
}

/* Add these new styles */
.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.3s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
</style> 