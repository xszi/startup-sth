<template>
  <div class="">火星seo</div>
  <div>
    title标签：主要是为了告诉搜索引擎我们的网站标题是什么，然后搜索引擎才会根据你提供的的title给你打上tag，用户在搜索的时候才会搜索到你。
    meta标签：这个标签根据name的不同有很多中，和SEO相关的主要是name=description 和name=keywords
    这两种，如果不设置这两个标签，对SEO的效果就会有所影响。
  </div>
</template>

<script setup>
useHead({
  title: ' 焱暒',
  viewport: 'width=device-width,initial-scale=1,maximum-scale=1 ',
  charset: 'utf-8',
  meta: [
    { name: 'description', content: '火星人博客' },
    { name: 'keywords', content: '养猪专业户' }
  ]
})
</script>

<style scoped></style>
