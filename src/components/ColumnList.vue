<template>
  <ul>
    <li v-for="item in list" :key="item.id">
      <img :src="item.avatar" :alt="item.avatar" />
      <h5>{{ item.title }}</h5>
      <p>{{ item.description }}</p>
      <a href="#">进入专栏</a>
    </li>
  </ul>
</template>

<script setup lang="ts">
import { defineProps, PropType } from 'vue'

export interface ColumnProps {
  id: number,
  title: string,
  avatar: string,
  description: string
}

defineProps({
  list: {
    type: Array as PropType<ColumnProps[]>,
    required: true
  }
})

</script>
