<template>
  <el-menu 
    class="footer" default-active="1"
    mode="horizontal" :ellipsis=false>
    <el-menu-item index="1">
      <el-icon><House /></el-icon>
    </el-menu-item>
    <el-menu-item index="2">
      <el-icon><ChatRound /></el-icon>
    </el-menu-item>
    <el-menu-item index="3">
      <el-icon><Setting /></el-icon>
    </el-menu-item>
    <el-menu-item index="4">
      <el-icon><Menu /></el-icon>
    </el-menu-item>
  </el-menu>
</template>

<script setup lang="ts">

</script>

<style scoped lang="scss">
.footer {
  width: 100%;
  position: absolute;
  bottom: 0;

  display: flex;
  justify-content: space-around;

  height: 7.5vh;
  background-color: #fff;
  border-top: 1.5px solid #f0f0f0;
}
</style>