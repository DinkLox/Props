<script setup>
import Display from './Display.vue'
import { ref } from 'vue'
const res = ref([
  {
    id: 1,
    title: 'aye',
    views: 10.0,
    author: 'Loc'
  },
  {
    id: 2,
    title: 'ayee',
    views: 20.0,
    author: 'Locc'
  },
  {
    id: 3,
    title: 'aaye',
    views: 110.0,
    author: 'LLoc'
  }
])

console.log(res.value)
// })
</script>
<template>
  <span v-for="item in res">
    <Display :title="item.title" :author="item.author" :views="item.views" />
  </span>
</template>
<style></style>
