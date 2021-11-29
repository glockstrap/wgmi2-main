<template>
  <div>
    <v-btn @click="onBtnClick()" color="#FD5D91" x-large class="story-btn"
      ><slot></slot><span class="btn-text">{{ text }}</span></v-btn
    >
    <v-snackbar v-model="snackbar" shaped color="#FD5D91">
      Address copied on the clipboard!

      <template v-slot:action="{ attrs }">
        <v-btn color="white" text v-bind="attrs" @click="snackbar = false">
          <v-icon>mdi-close</v-icon>
        </v-btn>
      </template>
    </v-snackbar>
  </div>
</template>

<script>
export default {
  props: ["text", "hreflink"],
  data: () => {
    return {
      snackbar: false,
    };
  },
  methods: {
    onBtnClick() {
      this.snackbar = true;
      navigator.clipboard.writeText(
        "0x20f6a313cb250062331fe70b9567e3ee5f01888b"
      );
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