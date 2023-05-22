<script>
export default {
  props: {
    urlImage: String,
    title: String,
  },
};
</script>

<template>
  <div class="card">
    <div class="img_container">
      <img :src="urlImage" :alt="title" />
    </div>
    <div class="text_container">
      <p class="title">{{ title.toUpperCase() }}</p>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: calc((100% / 6) - 1rem);
  margin: 1.5rem 0.5rem;
  .img_container {
    width: 100%;
    height: 100%;
    aspect-ratio: 1 / 1;
    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
    }
  }
  .text_container {
    color: white;
    font-size: 0.9em;
    text-align: center;
    margin-top: 0.3rem;
  }
}
.card:hover {
  cursor: pointer;
  opacity: 0.5;
}
</style>
