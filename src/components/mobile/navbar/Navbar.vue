<template>
  <v-app-bar color="#34FBEB" min-height="70px" max-height="70px" fixed tile class="pt-2">
    <v-img max-width="30" max-height="30" src="../../../assets/wgmi-coin.svg"></v-img>
    <v-spacer></v-spacer>
    <!-- <navbar-button text="The story" />
    <navbar-button text="Our community" />
    <navbar-button text="Join the movement" /> -->
    <navbar-icons filename="discord.svg" :hreflink="DISCORD_URL"/>
    <navbar-icons filename="twitter.svg" hreflink="https://twitter.com/wgmi4thepeople"/>
    <navbar-icons filename="telegram.svg" hreflink="https://t.me/WGMI_chan"/>
    <navbar-icons filename="coingecko.png" hreflink="https://www.coingecko.com/en/coins/wgmi"/>
    <navbar-icons filename="cmc.svg" hreflink="https://coinmarketcap.com/currencies/wgmi/"/>
  </v-app-bar>
</template>

<script>
// import NavbarButton from "./NavbarButton.vue";
import NavbarIcons from "./NavbarIcons.vue";
import { DISCORD_URL } from '@/config/constant.js'
export default {
  components: { NavbarIcons },
  // components: { NavbarButton, NavbarIcons },
  data: () => {
    return {
      DISCORD_URL: DISCORD_URL
    }
  }
};
</script>

<style>
</style>