<template>
  <figure class="p-6 text-center">
    <img class="w-32 h-32 rounded-full mx-auto" :src="image" alt="profile picture" width="32" height="32">
    <figcaption class="font-medium pt-6">
      <div class="text-cyan-900 text-xl">{{title}}</div>
      <div class="text-gray-500 font-light">{{subtitle}}</div>
    </figcaption>
    <blockquote><p class="text-lg pt-4 font-medium">{{headline}}</p></blockquote>
  </figure>
</template>

<script setup>
  const {title, subtitle, headline, image} = defineProps(['title', 'subtitle', 'headline', 'image'])
</script>