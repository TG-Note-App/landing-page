<template>
    <div class="space-y-4 sm:space-y-6">
        <h3 class="text-2xl sm:text-3xl font-bold">
            <span class="bg-gradient-to-r from-blue-400 via-purple-400 to-blue-400 text-transparent bg-clip-text">
                {{ title }}
            </span>
        </h3>
        <p class="text-gray-300 text-base sm:text-lg leading-relaxed">
            {{ description }}
        </p>
        <ul class="space-y-3 sm:space-y-4">
        <li v-for="(item, index) in items" 
            :key="index" 
            class="group flex items-center gap-2 sm:gap-3 p-2 sm:p-3 bg-white/5 rounded-lg sm:rounded-xl hover:bg-white/10 transition-all">
            <div :class="`w-8 sm:w-10 h-8 sm:h-10 rounded-lg bg-${item.iconColor}-500/20 flex items-center justify-center group-hover:scale-110 transition-transform`">
                <i :class="`fas ${item.icon} text-${item.iconColor}-400 group-hover:text-${item.iconColor}-300 text-sm sm:text-base`"></i>
            </div>
            <span class="text-gray-300 text-sm sm:text-base group-hover:text-white transition-colors">{{ item.text }}</span>
        </li>
        </ul>
    </div>
</template>

<script setup lang="ts">
interface ListItem {
  icon: string;
  iconColor: string;
  text: string;
}

interface Props {
  title: string;
  description: string;
  items: ListItem[];
}

defineProps<Props>();
</script>

<style>

</style>