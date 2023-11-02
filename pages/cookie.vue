<template>
  <h1>Counter:{{ counter }}</h1>
  <button @click="reset">Reset</button>
  <button @click="add">Add</button>
  <div>
    什么是HttpOnly？
    HttpOnly是包含在http返回头Set-Cookiew里面的一个附件的flag，所以它是后端服务器对cookie设置的一个附件属性，在生成cookie时使用HttpOnly标志有助于减轻客户端脚本访问收保护cookie的风险。
  </div>
  <div>
    还有maxAge/expires和secure的设置（这是一个安全设置，如果你的网址不是HTTPS的，并且把secure的值设置为true，那Cookie的值就不会传递给服务端。总的来说还是一个为了服务器安全的设置。）
  </div>
</template>

<script setup>
const counter = useCookie('counter', {
  htttpOnly: true
})
counter.value = counter.value || 0
const reset = () => {
  counter.value = 0
}
const add = () => {
  counter.value = counter.value + 1
}
</script>

<style scoped></style>
