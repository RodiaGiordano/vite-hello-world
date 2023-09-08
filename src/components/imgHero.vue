<script>
export default {
  data() {
    return {
      imgHero: "vue.svg",
    };
  },

  methods: {
    imgVite(img) {
      return new URL(`../assets/${img}`, import.meta.url).href;
    },
  },
};
</script>

<template>
  <img :src="imgVite(imgHero)" alt="" />
</template>

<style></style>
