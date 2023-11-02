<template>
  <div class="">获取的id:{{ $route.params.id }}</div>
</template>

<script setup>
import { ref } from 'vue'
const route = useRoute()
const id = ref(route.params.id)
console.log(id, 'kkkk')
</script>

<style scoped></style>
