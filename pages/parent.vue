<template>
  <div class="">Parent Page</div>
  <!-- 子页面的出口-->
  <p><NuxtLink to="/parent/child">child</NuxtLink></p>
  <p><NuxtLink to="/parent/child2">child2</NuxtLink></p>
  <NuxtPage />
</template>

<script setup>
import {} from 'vue'
</script>

<style scoped></style>
