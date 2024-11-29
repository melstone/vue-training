<script setup lang="ts">
import { RouterView } from 'vue-router'
import AppHeader from '@/components/AppHeader.vue'
import AppFooter from '@/components/AppFooter.vue'
</script>

<template>
  <AppHeader is-dark />

  <main class="main" role="main">
    <RouterView />
  </main>

  <AppFooter />
</template>
