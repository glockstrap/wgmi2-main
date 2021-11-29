<template>
<div>
  <navbar/>
   <head-img/>
   <story/>
</div>
</template>

<script>
import HeadImg from './head-img/HeadImg.vue';
import Navbar from './navbar/Navbar.vue';
import Story from './story/Story.vue';

export default {
  components: {
    Navbar,
    HeadImg,
    Story
  },
}
</script>

<style>

</style>