<template>
  <div>hello world</div>
</template>

<script setup>
import {} from 'vue'
const res = await useAsyncData('getList', () => $fetch('http://121.36.81.61:8000/getTenArticleList'))
console.log(res)
const res1 = await useFetch('http://121.36.81.61:8000/getTenArticleList')
const list = ref(res1.data._rawValue.data)
console.log(list)
</script>

<style scoped></style>
