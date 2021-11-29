<template>
  <div style="background-color: black; margin-bottom: -100px; margin-top: 70px">
    <div>
      <img width="100%" :src="require(`@/assets/mobile-hero-art.png`)" @load="scrollToTop" />
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    scrollToTop() {
      window.scroll({
        top: 0,
        left: 0,
        behavior: "smooth",
      });
    },
  },
  mounted() {
    this.scrollToTop()
  }
};
</script>

<style>
</style>