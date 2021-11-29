<template>
  <div>
    <navbar />
    <head-img />
    <story/>
  </div>
</template>

<script>
import Navbar from "./navbar/Navbar.vue";
import HeadImg from "./head-img/HeadImg.vue";
import Story from './story/Story.vue';

export default {
  components: {
    HeadImg,
    Navbar,
    Story,
  },
};
</script>

<style>
</style>