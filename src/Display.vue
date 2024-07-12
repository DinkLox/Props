<script setup>
const props = defineProps(['title', 'author', 'views'])
</script>
<template>
  <div class="container">
    <div class="item">
      <img src="https://img.youtube.com/vi/dQw4w9WgXcQ/0.jpg" alt="Image 1" />
      <div class="title">{{ props.title }}</div>
      <div class="author">{{ props.author }}</div>
      <div class="views">{{ props.views }}</div>
    </div>
  </div>
</template>
<style scoped>
body {
  font-family: Arial, sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  height: 100vh;
  margin: 0;
}
.container {
  display: grid;
  grid-template-columns: repeat(5, 1fr);
  grid-gap: 10px;
  width: 80%;
}
.item {
  text-align: center;
}
.item img {
  width: 100%;
  height: 100px; /* Đặt chiều cao cố định */
  object-fit: cover; /* Giữ tỉ lệ hình ảnh */
  display: block;
}
.title {
  font-weight: bold;
  margin: 5px 0;
}
.author {
  color: gray;
  margin: 3px 0;
}
.views {
  color: darkblue;
  margin: 3px 0;
}
</style>
