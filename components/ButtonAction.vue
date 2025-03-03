<template>
  <a :href="link" target="_blank" class="animate-fade-left animate-once animate-ease-out flex items-start rounded-lg border border-gray-400 bg-white text-gray-900 px-5 py-4 text-lg leading-6 font-medium shadow-md hover:shadow-xl transition ease-in-out duration-150 dark:bg-gray-800 dark:text-white dark:border-gray-600 dark:hover:shadow-2xl">
    <p class="mr-3 h-6 w-6">{{icon}}</p>
    {{text}}
  </a>
</template>

<script setup>
const {link, icon, text} = defineProps(['link', 'icon', 'text'])
</script>