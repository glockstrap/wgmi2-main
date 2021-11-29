<template>
  <v-app>
    <div v-if="!isMobile()">
      <desktop />
    </div>
    <div v-else>
      <mobile />
    </div>
  </v-app>
</template>

<script>
import Desktop from "./components/desktop/Desktop.vue";
import Mobile from "./components/mobile/Mobile.vue";

export default {
  name: "App",

  components: {
    Desktop,
    Mobile,
  },
  methods: {

    isMobile() {
      if (
        /Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(
          navigator.userAgent
        )
      ) {
        return true;
      } else {
        return false;
      }
    },
  },

};
</script>
<style>
html,
body {
  overflow-x: hidden;
}
</style>