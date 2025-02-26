<template>
    <div class="mb-24 mt-24 relative" id="features-overview">
        <!-- Background Effects -->
        <div class="absolute -z-10 top-1/2 -left-20 w-60 h-60 bg-blue-500/10 rounded-full blur-3xl"></div>
        <div class="absolute -z-10 bottom-0 right-0 w-60 h-60 bg-purple-500/10 rounded-full blur-3xl"></div>

        <div class="text-center mb-16">
            <h2 class="text-4xl font-bold mb-6">
            <span class="bg-gradient-to-r from-blue-400 via-purple-400 to-blue-400 text-transparent bg-clip-text">
                Everything You Need in One Place
            </span>
            </h2>
            <p class="text-xl text-gray-300">From quick notes to complex organization - we've got you covered</p>
        </div>

        <div class="grid md:grid-cols-2 gap-8">
            <!-- Left Column: Features List -->
            <div class="space-y-6">
            <div class="group p-6 bg-gray-900/40 rounded-2xl backdrop-blur-xl border border-white/10 hover:border-white/20 transition-all">
                <div class="flex items-start gap-4">
                <div class="w-12 h-12 rounded-xl bg-blue-500/20 flex items-center justify-center shrink-0 group-hover:scale-110 transition-transform">
                    <i class="fas fa-wand-magic-sparkles text-blue-400"></i>
                </div>
                <div>
                    <h3 class="text-xl font-semibold text-white mb-2">Smart Organization</h3>
                    <p class="text-gray-400">AI-powered categorization automatically sorts your notes into relevant folders and tags.</p>
                </div>
                </div>
            </div>

            <div class="group p-6 bg-gray-900/40 rounded-2xl backdrop-blur-xl border border-white/10 hover:border-white/20 transition-all">
                <div class="flex items-start gap-4">
                <div class="w-12 h-12 rounded-xl bg-purple-500/20 flex items-center justify-center shrink-0 group-hover:scale-110 transition-transform">
                    <i class="fas fa-magnifying-glass text-purple-400"></i>
                </div>
                <div>
                    <h3 class="text-xl font-semibold text-white mb-2">Powerful Search</h3>
                    <p class="text-gray-400">Find any note instantly with our advanced search capabilities and smart filters.</p>
                </div>
                </div>
            </div>

            <div class="group p-6 bg-gray-900/40 rounded-2xl backdrop-blur-xl border border-white/10 hover:border-white/20 transition-all">
                <div class="flex items-start gap-4">
                <div class="w-12 h-12 rounded-xl bg-green-500/20 flex items-center justify-center shrink-0 group-hover:scale-110 transition-transform">
                    <i class="fas fa-share-nodes text-green-400"></i>
                </div>
                <div>
                    <h3 class="text-xl font-semibold text-white mb-2">Easy Sharing</h3>
                    <p class="text-gray-400">Share notes with friends or save them for yourself - all within Telegram</p>
                </div>
                </div>
            </div>
            </div>

            <!-- Right Column: Interactive Preview -->
            <div class="relative">
            <div class="absolute inset-0 bg-gradient-to-r from-blue-500/10 via-purple-500/10 to-blue-500/10 rounded-3xl blur-xl"></div>
            <div class="relative bg-gray-900/40 rounded-3xl p-8 backdrop-blur-xl border border-white/10">
                <div class="space-y-6">
                <div class="flex items-center justify-between mb-5">
                    <div class="flex items-center gap-3">
                    <div class="w-10 h-10 rounded-xl bg-blue-500/20 flex items-center justify-center">
                        <i class="fas fa-folder text-blue-400"></i>
                    </div>
                    <span class="text-lg font-medium text-white">Notes</span>
                    </div>
                    <div class="flex gap-2">
                    <button class="w-8 h-8 rounded-lg bg-white/5 flex items-center justify-center hover:bg-white/10 transition-all">
                        <i class="fas fa-list text-white/60"></i>
                    </button>
                    </div>
                </div>

                <!-- Note Items -->
                <div class="space-y-2">
                    <!-- Note 1 -->
                    <div class="group relative">
                    <div class="absolute inset-0 bg-gradient-to-r from-blue-500/20 via-purple-500/20 to-blue-500/20 rounded-lg blur-sm opacity-0 group-hover:opacity-100 transition duration-300"></div>
                        <div class="relative p-3 bg-white/5 rounded-lg hover:bg-white/10 transition-all border border-white/10 group-hover:border-white/20">
                        <div class="flex items-start gap-3">
                            <div class="shrink-0">
                            <div class="w-8 h-8 rounded-lg bg-gradient-to-br from-blue-500/20 to-purple-500/20 flex items-center justify-center group-hover:scale-110 transition-transform">
                                <i class="fas fa-code text-blue-400 group-hover:text-blue-300 text-sm"></i>
                            </div>
                            </div>
                            <div class="flex-1 min-w-0">
                            <div class="flex items-center justify-between">
                                <h4 class="text-white text-sm font-medium truncate">API Integration</h4>
                                <span class="text-xs text-white/40">2m ago</span>
                            </div>
                            <p class="text-xs text-gray-400 line-clamp-1 my-1">Implementation steps...</p>
                            <div class="flex items-center gap-2">
                                <span class="px-1.5 py-0.5 text-xs rounded-full bg-blue-500/10 text-blue-400 border border-blue-500/20">#code</span>
                                <span class="px-1.5 py-0.5 text-xs rounded-full bg-purple-500/10 text-purple-400 border border-purple-500/20">#api</span>
                            </div>
                            </div>
                        </div>
                        </div>
                    </div>

                    <!-- Note 2 -->
                    <div class="group relative">
                        <div class="absolute inset-0 bg-gradient-to-r from-green-500/20 via-emerald-500/20 to-green-500/20 rounded-lg blur-sm opacity-0 group-hover:opacity-100 transition duration-300"></div>
                        <div class="relative p-3 bg-white/5 rounded-lg hover:bg-white/10 transition-all border border-white/10 group-hover:border-white/20">
                        <div class="flex items-start gap-3">
                            <div class="shrink-0">
                            <div class="w-8 h-8 rounded-lg bg-gradient-to-br from-green-500/20 to-emerald-500/20 flex items-center justify-center group-hover:scale-110 transition-transform">
                                <i class="fas fa-list-check text-green-400 group-hover:text-green-300 text-sm"></i>
                            </div>
                            </div>
                            <div class="flex-1 min-w-0">
                            <div class="flex items-center justify-between">
                                <h4 class="text-white text-sm font-medium truncate">Project Plan</h4>
                                <span class="text-xs text-white/40">1h ago</span>
                            </div>
                            <p class="text-xs text-gray-400 line-clamp-1 my-1">Q1 Goals: 1. Launch beta...</p>
                            <div class="flex items-center gap-2">
                                <span class="px-1.5 py-0.5 text-xs rounded-full bg-green-500/10 text-green-400 border border-green-500/20">#plan</span>
                                <span class="px-1.5 py-0.5 text-xs rounded-full bg-emerald-500/10 text-emerald-400 border border-emerald-500/20">#goals</span>
                            </div>
                            </div>
                        </div>
                        </div>
                    </div>

                    <!-- Note 3 -->
                    <div class="group relative">
                        <div class="absolute inset-0 bg-gradient-to-r from-orange-500/20 via-yellow-500/20 to-orange-500/20 rounded-lg blur-sm opacity-0 group-hover:opacity-100 transition duration-300"></div>
                        <div class="relative p-3 bg-white/5 rounded-lg hover:bg-white/10 transition-all border border-white/10 group-hover:border-white/20">
                        <div class="flex items-start gap-3">
                            <div class="shrink-0">
                            <div class="w-8 h-8 rounded-lg bg-gradient-to-br from-orange-500/20 to-yellow-500/20 flex items-center justify-center group-hover:scale-110 transition-transform">
                                <i class="fas fa-lightbulb text-orange-400 group-hover:text-orange-300 text-sm"></i>
                            </div>
                            </div>
                            <div class="flex-1 min-w-0">
                            <div class="flex items-center justify-between">
                                <h4 class="text-white text-sm font-medium truncate">Feature Ideas</h4>
                                <span class="text-xs text-white/40">3h ago</span>
                            </div>
                            <p class="text-xs text-gray-400 line-clamp-1 my-1">Improvements for v2...</p>
                            <div class="flex items-center gap-2">
                                <span class="px-1.5 py-0.5 text-xs rounded-full bg-orange-500/10 text-orange-400 border border-orange-500/20">#ideas</span>
                                <span class="px-1.5 py-0.5 text-xs rounded-full bg-yellow-500/10 text-yellow-400 border border-yellow-500/20">#ui</span>
                            </div>
                            </div>
                        </div>
                        </div>
                    </div>
                </div>

                <!-- Quick Actions -->
                <div class="pt-4 border-t border-white/10">
                    <div class="flex gap-4">
                    <button class="flex-1 px-4 py-2 bg-blue-500/10 rounded-lg text-blue-400 hover:bg-blue-500/20 transition-all">
                        <i class="fas fa-plus mr-2"></i>New Note
                    </button>
                    <button class="flex-1 px-4 py-2 bg-purple-500/10 rounded-lg text-purple-400 hover:bg-purple-500/20 transition-all">
                        <i class="fas fa-folder-plus mr-2"></i>New Folder
                    </button>
                    </div>
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