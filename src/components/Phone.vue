<template>
    <div class="relative w-[320px] h-[640px] bg-gradient-to-b from-[#1A1A1A] to-black rounded-[2.5rem] p-3 shadow-2xl">
        <!-- Screen Content -->
        <div class="relative h-full w-full bg-gradient-to-br from-[#0A0A0A] to-[#1A1A1A] rounded-[2.25rem] overflow-hidden border border-white/10">
            <!-- Ambient Light Effect -->
            <div class="absolute inset-0 bg-gradient-to-t from-blue-500/5 to-transparent"></div>
            
            <!-- Main Content -->
            <div class="h-full w-full relative">
                <!-- Status Bar -->
                <div class="px-5 pt-3 pb-2 flex justify-between items-center text-xs text-white/60">
                    <span>9:41</span>
                    <div class="flex items-center gap-2">
                        <i class="fas fa-wifi"></i>
                        <i class="fas fa-battery-full"></i>
                    </div>
                </div>

                <slot></slot>
            </div>
        </div>
    </div>
</template>

<script setup lang="ts">

</script>

<style>

</style>