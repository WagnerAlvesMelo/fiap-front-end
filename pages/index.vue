<template>
  <main class="max-w-xs mx-auto h-full space-y-6">
    <ToggleDarkMode/>
    <ProfileInfo
        title="Wagner"
        subtitle="@wagner.melo13"
        headline="Software Engineer | Front-End"
        image="/img/me.enc"
    />
    <ButtonAction
        v-for="(button, idx) in buttons"
        :key="button.link"
        :link="button.link"
        :icon="button.icon"
        :text="button.text"
        :style="{ animationDelay: `${idx * 100}ms` }"
    />
  </main>
</template>

<script setup lang="ts">

const themeCookie = useCookie('theme');
const isDarkMode = themeCookie.value === 'dark';

useHead({
  htmlAttrs: {
    class: {
      'bg-white dark:bg-gray-800': true,
      dark: isDarkMode
    }
  },
});
const buttons = [
  { link: 'https://www.linkedin.com/in/wagner-alves-603ba0163/', icon: '🔗', text: 'LinkedIn' },
  { link: 'https://github.com/WagnerAlvesMelo', icon: '🐙', text: 'Github' },
  { link: 'https://wa.me/5511980734917', icon: '💬', text: 'WhatsApp' },
  { link: 'https://www.instagram.com/wagner.melo13/', icon: '📸', text: 'Instagram' },
];
</script>
