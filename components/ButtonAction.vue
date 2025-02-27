<template>
  <a :href="link" target="_blank" class="flex items-start rounded-lg border border-gray-400 bg-white px-5 py-4 text-lg leading-6 font-medium shadow-md hover:shadow-xl transition ease-in-out duration-150">
    <p class="mr-3 h-6 w-6">{{icon}}</p>
    {{text}}
  </a>
</template>
<script setup>
  const {link, icon, text} = defineProps(['link', 'icon', 'text'])
</script>