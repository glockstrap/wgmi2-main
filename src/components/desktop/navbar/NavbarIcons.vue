<template>
  <v-btn icon class="mx-3" @click="onBtnClick()">
      <v-img
        max-height="40"
        max-width="40"
        :src="require(`@/assets/${filename}`)">
      </v-img>
      
    </v-btn>
</template>

<script>
export default {
    props: ["filename", "hreflink"],
    methods: {
      onBtnClick() {
      window.open(this.hreflink, "_blank");
      }
    }
}
</script>

<style>

</style>