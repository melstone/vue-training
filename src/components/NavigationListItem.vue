<script lang="ts" setup>
import { toRefs } from 'vue';

interface IItem {
  text: string
  to: string
}

interface Props {
  item: IItem
}

const props = defineProps<Props>()

const { item } =  toRefs(props)
</script>

<template>
  <li class="header-nav__item">
    <RouterLink class="header-nav__link" :to="item.to">{{ item.text }}</RouterLink>
  </li>
</template>
