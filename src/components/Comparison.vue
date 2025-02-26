<template>
    <div class="mb-24 mt-24" id="comparison">
        <h2 class="text-3xl font-bold text-center mb-12">
            <span class="bg-gradient-to-r from-blue-400 to-purple-400 text-transparent bg-clip-text">Why Switch to Telegram Mini-App Notes?</span>
        </h2>
        
        <div class="relative">
        <!-- Background Glow Effects -->
        <div class="absolute -z-10 top-1/2 -left-20 w-60 h-60 bg-blue-500/10 rounded-full blur-3xl"></div>
        <div class="absolute -z-10 bottom-0 right-0 w-60 h-60 bg-purple-500/10 rounded-full blur-3xl"></div>
        
        <!-- Main Content -->
        <div class="relative bg-gray-800/30 rounded-2xl p-8 backdrop-blur-xl border border-white/5">
            <div class="grid md:grid-cols-2 gap-12">
            <!-- Traditional Apps Column -->
            <div class="relative group">
                <div class="absolute inset-0 bg-gradient-to-b from-red-500/5 to-transparent rounded-xl transition-all duration-300 group-hover:from-red-500/10"></div>
                <div class="relative p-6">
                <div class="flex items-center gap-4 mb-8">
                    <div class="w-12 h-12 rounded-xl bg-red-500/10 flex items-center justify-center">
                    <i class="fas fa-mobile-screen-button text-red-400 text-xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-red-400">Traditional Note Apps</h3>
                </div>
                <ul class="space-y-6">
                    <!-- List items with enhanced styling -->
                    <li class="flex items-center gap-4 group/item">
                    <div class="w-8 h-8 rounded-full bg-red-500/10 flex items-center justify-center group-hover/item:bg-red-500/20 transition-all">
                        <i class="fas fa-times text-red-400 text-sm"></i>
                    </div>
                    <span class="text-gray-400 group-hover/item:text-gray-300 transition-colors">Separate app to install</span>
                    </li>
                    <li class="flex items-center gap-4 group/item">
                    <div class="w-8 h-8 rounded-full bg-red-500/10 flex items-center justify-center group-hover/item:bg-red-500/20 transition-all">
                        <i class="fas fa-times text-red-400 text-sm"></i>
                    </div>
                    <span class="text-gray-400 group-hover/item:text-gray-300 transition-colors">Complex setup process</span>
                    </li>
                    <li class="flex items-center gap-4 group/item">
                    <div class="w-8 h-8 rounded-full bg-red-500/10 flex items-center justify-center group-hover/item:bg-red-500/20 transition-all">
                        <i class="fas fa-times text-red-400 text-sm"></i>
                    </div>
                    <span class="text-gray-400 group-hover/item:text-gray-300 transition-colors">Limited sharing options</span>
                    </li>
                </ul>
                </div>
            </div>

            <!-- Smart Notes Column -->
            <div class="relative group">
                <div class="absolute inset-0 bg-gradient-to-b from-green-500/5 to-transparent rounded-xl transition-all duration-300 group-hover:from-green-500/10"></div>
                <div class="relative p-6">
                <div class="flex items-center gap-4 mb-8">
                    <div class="w-12 h-12 rounded-xl bg-green-500/10 flex items-center justify-center">
                    <i class="fas fa-rocket text-green-400 text-xl"></i>
                    </div>
                    <h3 class="text-xl font-semibold text-green-400">Telegram Mini-App Notes</h3>
                </div>
                <ul class="space-y-6">
                    <!-- List items with enhanced styling -->
                    <li class="flex items-center gap-4 group/item"> 
                    <div class="w-8 h-8 rounded-full bg-green-500/10 flex items-center justify-center group-hover/item:bg-green-500/20 transition-all">
                        <i class="fas fa-check text-green-400 text-sm"></i>
                    </div>
                    <span class="text-gray-300 group-hover/item:text-white transition-colors">Works right in Telegram</span>
                    </li>
                    <li class="flex items-center gap-4 group/item">
                    <div class="w-8 h-8 rounded-full bg-green-500/10 flex items-center justify-center group-hover/item:bg-green-500/20 transition-all">
                        <i class="fas fa-check text-green-400 text-sm"></i>
                    </div>
                    <span class="text-gray-300 group-hover/item:text-white transition-colors">Start using instantly</span>
                    </li>
                    <li class="flex items-center gap-4 group/item">
                    <div class="w-8 h-8 rounded-full bg-green-500/10 flex items-center justify-center group-hover/item:bg-green-500/20 transition-all">
                        <i class="fas fa-check text-green-400 text-sm"></i>
                    </div>
                    <span class="text-gray-300 group-hover/item:text-white transition-colors">Share notes with one click</span>
                    </li>
                </ul>
                </div>
            </div>
            </div>
        </div>
        </div>
    </div>
</template>

<script setup lang="ts">

</script>

<style>

</style>