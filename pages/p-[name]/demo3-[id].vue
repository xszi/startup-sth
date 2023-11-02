<template>
  <div class="">获取的id:{{ $route.params.name }}</div>
  <div class="">获取的id:{{ $route.params.id }}</div>
</template>

<script setup>
import { ref } from 'vue'
const route = useRoute()
const name = ref(route.params.name)
const id = ref(route.params.id)
console.log(name, id, 'kkkk')
</script>

<style scoped></style>
