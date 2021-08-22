<template>
  <ColumnList :list="data"></ColumnList>
</template>

<script setup lang="ts">
import ColumnList, { ColumnProps } from './components/ColumnList.vue'

const data: ColumnProps[] = [
  {
    id: 1,
    title: 'test1',
    description: 'description1',
    avatar: 'https://cdn.jsdelivr.net/gh/pys1992/storage@main/20210820005347.png'
  },
  {
    id: 2,
    title: 'test2',
    description: 'description2',
    avatar: 'https://cdn.jsdelivr.net/gh/pys1992/storage@main/20210820005347.png'
  },
  {
    id: 3,
    title: 'test3',
    description: 'description3',
    avatar: 'https://cdn.jsdelivr.net/gh/pys1992/storage@main/20210820005347.png'
  }
]
</script>
