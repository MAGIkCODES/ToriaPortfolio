<script setup>
import { RouterLink, RouterView } from 'vue-router'
// import TheWelcome from './components/TheWelcome.vue'
import navBar from './components/navBar.vue'
import FooterView from './views/FooterView.vue';
</script>

<template>
  <navBar />
  <RouterView />

  <FooterView />
</template>

