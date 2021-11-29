<template>
      <v-btn class="btn" text>{{text}}</v-btn>

</template>

<script>
export default {
    props: ["text"]
}
</script>

<style>
.btn {
  color: #000000;
  text-shadow: -2px 1px #ffffff, -3px 5px #ffffff, 1px 0 #ffffff, 0 -1px #ffffff;
  font-size: 1.5rem !important;
}
</style>