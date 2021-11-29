<template>
  <v-app-bar color="#34FBEB" min-height="90px" max-height="90px" fixed class="pt-6 px-12">
    <v-img max-width="60" max-height="60" src="../../../assets/wgmi-coin.svg"></v-img>
    <v-spacer></v-spacer>
    <!-- <navbar-button text="The story" />
    <navbar-button text="Our community" />
    <navbar-button text="Join the movement" /> -->
    <navbar-icons filename="discord.svg" :hreflink="DISCORD_URL"/>
    <navbar-icons filename="twitter.svg" hreflink="https://twitter.com/wgmi4thepeople"/>
    <navbar-icons filename="telegram.svg" hreflink="https://t.me/WGMI_chan"/>
    <navbar-icons filename="coingecko.png" hreflink="https://www.coingecko.com/en/coins/wgmi"/>
    <navbar-icons filename="cmc.svg" hreflink="https://coinmarketcap.com/currencies/wgmi/"/>
    <!-- <navbar-icons filename="dextools.png" hreflink="https://www.dextools.io/app/ether/pair-explorer/0xa38400a9b62e383170500096271ee3f727de2489"/> -->
  </v-app-bar>
</template>

<script>
// import NavbarButton from "./NavbarButton.vue";
import NavbarIcons from "./NavbarIcons.vue";
import { DISCORD_URL } from '@/config/constant.js'
export default {
  components: { NavbarIcons },
  data: () => {
    return {
      DISCORD_URL: DISCORD_URL
    }
  }
};
</script>

<style>
</style>