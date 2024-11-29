<script lang="ts" setup>
import NavigationListItem from './NavigationListItem.vue'

const links = [
  {
    text: 'Home',
    to: '/'
  },
  {
    text: 'About',
    to: '/about'
  },
  {
    text: 'Contact',
    to: '/contact'
  }
]
</script>

<template>
  <ul class="header-nav__list">
    <NavigationListItem
      v-for="(link, index) in links"
      :key="index"
      :item="link"
    />
  </ul>
</template>

<style scoped>
</style>
