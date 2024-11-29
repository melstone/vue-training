<script lang="ts" setup>
import { toRefs } from 'vue';
import NavigationList from './NavigationList.vue'

interface Props {
  isDark: boolean
}

const props = defineProps<Props>()

const { isDark } =  toRefs(props)
</script>

<template>
  <header :class="['header', { 'is-dark': isDark }]">
    <div class="header__logo" />
    <nav role="navigation" class="header-nav">
      <NavigationList />
    </nav>
  </header>
</template>

<style scoped>
.header {
  padding: 1rem;
  background-color: #eee;
  display: flex;
  align-items: center;
}

.is-dark {
  background-color: #000;
}
</style>
