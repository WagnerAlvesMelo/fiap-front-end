<template>
  <div class="flex items-center justify-end space-x-4 p-4">
    <button @click="toggleDarkMode" class="cursor-pointer dark:text-white text-black">
      <span v-if="isDarkMode">Light Mode ☀️</span>
      <span v-else>Dark Mode 🌙</span>
    </button>
  </div>
</template>

<script setup>
import { ref } from 'vue';
import { useCookie } from '#app';

const themeCookie = useCookie('theme');
const isDarkMode = ref(themeCookie.value === 'dark');

const toggleDarkMode = () => {
  isDarkMode.value = !isDarkMode.value;
  themeCookie.value = isDarkMode.value ? 'dark' : 'light';

  document.documentElement.classList.toggle('dark', isDarkMode.value);
};
</script>
