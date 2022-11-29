<template>
<div class="posts">
  <Post></Post>
  <Post></Post>
  <Post></Post>
  <Post></Post>
  <Post></Post>
  <Post></Post>
  <Post></Post>
</div>
</template>

<script setup lang="ts">
import Post from './Post.vue'
</script>

<style scoped lang="scss">
.posts {
  height: 86vh;
  overflow-y: scroll;
}

/* Hide scrollbar for Chrome, Safari and Opera */
.posts::-webkit-scrollbar {
    display: none;
}
/* Hide scrollbar for IE, Edge and Firefox */
.posts {
  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
}
</style>