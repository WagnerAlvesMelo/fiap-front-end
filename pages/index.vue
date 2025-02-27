<template>
  <ProfileInfo
      title="Wagner"
      subtitle="@wagner.melo13"
      headline="Software Engineer | Front-End"
      image="/img/me.enc"
  />
  <main class="max-w-xs mx-auto space-y-6">
    <ButtonAction
        v-for="(button) in buttons"
        :key="button.link"
        :link="button.link"
        :icon="button.icon"
        :text="button.text"
    />
  </main>
</template>

<script setup lang="ts">
const buttons = [
  { link: 'https://www.linkedin.com/in/wagner-alves-603ba0163/', icon: '🔗', text: 'LinkedIn' },
  { link: 'https://github.com/WagnerAlvesMelo', icon: '🐙', text: 'Github' },
  { link: 'https://wa.me/5511980734917', icon: '💬', text: 'WhatsApp' },
  { link: 'https://www.instagram.com/wagner.melo13/', icon: '📸', text: 'Instagram' },
];
</script>
