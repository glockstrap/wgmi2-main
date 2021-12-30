<template>
  <v-btn @click="onBtnClick()" color="#FD5D91" x-large class="story-btn"
    ><slot></slot><span class="btn-text">{{ text }}</span></v-btn
  >
</template>

<script>
export default {
  props: ["text", "hreflink"],
  methods: {
    onBtnClick() {
      window.open(this.hreflink, "_blank");
    },
  },
};
</script>

<style scoped>
.story-btn {
  padding: 3rem;
  box-shadow: -10px 10px #193be3;
}

.btn-text {
  font-size: 2rem;
  color: white;
}
</style>