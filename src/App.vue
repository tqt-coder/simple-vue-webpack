<template>
  <div class="app">
    <h1>Hello {{ message }} V2 tqtuan5 update</h1>
    <h2>{{ count }}</h2>
    <button @click="handleAdd">+1</button>
    <button @click="handleDes">-1</button>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const count = ref<number>(0)
const message = 'vue'

const handleAdd = () => count.value++
const handleDes = () => count.value--
</script>

<style scoped lang="less">
.app {
  background-color: yellow;
  h1 {
    color: red;
    font-size: 50px;
  }
}
</style>
