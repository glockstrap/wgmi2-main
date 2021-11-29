<template>
  <v-img style="margin-top: 70px" :src="require(`@/assets/wgmi-bg.png`)" @load="scrollToTop"/>
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