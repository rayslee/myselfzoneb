<template>
  <div class="header">{{name}}</div>
</template>

<script setup lang="ts">
import { ref } from 'vue'

const name = ref("主页")
</script>

<style scoped lang="scss">
.header {
  width: 100%;
  text-align: center;
  line-height: 6.5vh;
  background-color: #fff;
  border-bottom: 1.5px solid #f0f0f0;
}
</style>