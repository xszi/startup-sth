<template>
  <div class="">
    <!-- 组件懒加载，只有组件在页面上显示的时候才去加载 -->
    <!-- 可以用来优化页面的打开速度，比如你有一个几百行的长列表。直接加载会给服务器造成很大压力，如果在其他内容已经完成后，过1-2秒再加载这个长列表，就会给用户很好的体验。也会减少服务器的压力。 -->
    <lazyText v-if="show" />
    <button @click="handleClick">显示/隐藏</button>
  </div>
</template>

<script setup>
import { ref } from 'vue'
const show = ref(false)
const handleClick = () => {
  show.value = show.value ? false : true
}
</script>

<style scoped></style>
