<script>
export default {
  data() {
    return {
      title: "My banner title",
      image: "milano.jpg",
    };
  },
  methods: {
    getImagePath(imageName) {
      return new URL(`../assets/img/${imageName}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <div class="banner">
    <h2>{{ title }}</h2>
    <img :src="getImagePath(image)" alt="" />
  </div>
</template>

<style>
.banner {
  position: relative;
}

.banner img {
  width: 100%;
}

.banner h2 {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  padding: 20px;
  background-color: rgba(0, 0, 0, 0.4);
  color: white;
}
</style>
