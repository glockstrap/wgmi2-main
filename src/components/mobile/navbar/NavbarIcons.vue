<template>
  <v-btn icon @click="onBtnClick()">
      <v-img
        max-height="15"
        max-width="15"
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