<template>
  <div>
    <v-container class="story-container-1 px-12" fluid>
      <v-row>
        <div style="text-align: center; font-size: 3rem" class="rosaviro">
          The story
        </div> </v-row
      ><v-row>
        <div class="inter-text">
          of $WGMI began on November 11, 2021, during its launch. It started off
          as a promising memecoin that touched upon a popular saying in the
          crypto/NFT space, WGMI, which means
          <span style="color: #34fbeb">"We're Gonna Make It"</span>. <br />
          <br />
          However, the investors' enthusiasm soon turned sour when it was
          realized that the developer held a majority share and sold all of his
          stakes, bringing the price of $WGMI down to
          <span style="color: #f92a68">almost zero</span>.
        </div>
      </v-row>
    </v-container>
    <v-container class="story-container-2 px-12" fluid>
      <v-row>
        <div class="img-container">
          <v-img
            class="img"
            :src="require(`@/assets/community-takeover-graphic.png`)"
          />
        </div>
      </v-row>
      <v-row style="margin-top: 50px">
        <div class="inter-text">
          The victims, however, did not submit to this attack on honest
          participants of the space. The victims got together to form a
          community and decided to take over the coin, bringing the market cap
          from $80,000.00 to
          <span style="color: #34fbeb">$30,000,000.00 within a day. </span
          ><br />
          <br />
          $WGMI is a story of how a small group of strong-headed individuals
          banded together to fight for what is right. All members of the
          community subscribe to the notion that, we will all truly make it.
        </div>
      </v-row>

      <v-container style="text-align: center; margin-top: 50px">
        <v-img
          max-width="100px"
          style="margin: 0 auto"
          :src="require(`@/assets/wgmi-vert.png`)"
        />
        <div class="rosaviro" style="font-size: 1.5rem">
          represents hope and optimism for those who need it the most.
        </div>
      </v-container>
    </v-container>
    <div class="whole-container-3">
      <v-container class="story-container-3 px-12" fluid>
        <v-row>
          <div class="community">
            Our community. <br />
            Built different. <br />
            From the ashes.
          </div>
        </v-row>
        <v-row>
          <div class="community-description-mobile inter-text">
            We’re 10<span class="community-description-text"
              >0% community driven. </span
            ><br />
            Rugger dev is gone and no longer
            <a
              href="https://etherscan.io/address/0xdca1893ab61a21f2413255d19e175d66ccd9fcad#tokentxns"
              target="_blank"
              >owns any $WGMI</a
            >
            or have
            <a
              href="https://tokensniffer.com/token/0x20f6a313cb250062331fe70b9567e3ee5f01888b"
              target="_blank"
            >
              ownership</a
            >
            of the contract.<br />
            <br />
            <br />
            This is for the P<span class="community-description-text pr-10 pt-2"
              >eople.</span
            >
            <br />
            This is f<span class="community-description-text pt-2"
              >or the Cultu</span
            >re.
          </div>
        </v-row>
      </v-container>
      <div class="mt-12">
        <v-img :src="require(`@/assets/screenshot1.png`)" />
      </div>
      <div class="mt-4">
        <v-img max-width="60%" :src="require(`@/assets/screenshot2.png`)" />
      </div>
      <div class="mt-4">
        <v-img
          style="margin-left: auto; margin-right: 0"
          max-width="70%"
          :src="require(`@/assets/screenshot3.png`)"
        />
      </div>
      <div class="mt-4">
        <v-img :src="require(`@/assets/screenshot4.png`)" />
      </div>
      <div class="mt-4 pl-3">
        <v-img max-width="70%" :src="require(`@/assets/screenshot5.png`)" />
      </div>
      <div class="mt-4 pr-3">
        <v-img
          style="margin-left: auto; margin-right: 0"
          max-width="70%"
          :src="require(`@/assets/screenshot6.png`)"
        />
      </div>
      <div class="mt-4 pl-3">
        <v-img :src="require(`@/assets/screenshot7.png`)" />
      </div>
      <v-container class="story-container-4">
        <v-row>
          <v-col>
            <div class="more-to-come">And more to come...</div>
          </v-col>
        </v-row>
        <v-row>
          <v-col class="btn-col">
            <story-button
              text="JOIN OUR DISCORD"
              :hreflink="DISCORD_URL"
              ><v-img
                max-height="40"
                max-width="40"
                :src="require(`@/assets/discord-white.svg`)"
                class="mr-2"
              >
              </v-img
            ></story-button>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <v-container fluid class="story-container-5">
      <v-row>
        <v-col class="btn-col">
          <copy-button
            text="COPY CONTRACT ADDRESS"
          />
        </v-col>
      </v-row>
      <v-row>
        <v-col class="btn-col">
          <story-button
            text="BUY ON UNISWAP"
            hreflink="https://app.uniswap.org/#/swap?outputCurrency=0x20f6a313cb250062331fe70b9567e3ee5f01888b&slippage=2"
          />
        </v-col>
      </v-row>
      <v-row>
        <v-col class="btn-col"
          ><v-img
            style="display: inline-block"
            class="mr-3"
            max-height="20px"
            max-width="20px"
            :src="require(`@/assets/attention-icon.svg`)"
          /><span style="font-size: 12px; text-align: left; color: #183ae0"
            >2% slippage recommended for Uniswap
          </span></v-col
        >
      </v-row>

      <v-row style="margin-top: 20px">
        <v-col class="btn-col">
          <story-button
            text="BUY ON MISTX"
            hreflink="https://app.mistx.io/#/exchange?outputCurrency=0x20f6a313cb250062331fe70b9567e3ee5f01888b"
          />
        </v-col>
      </v-row>
      <v-row style="margin-top: 30px">
        <v-col class="btn-col">
          <story-button
            text="BUY ON COWSWAP"
            hreflink="https://cowswap.exchange/#/swap?outputCurrency=0x20f6a313cb250062331fe70b9567e3ee5f01888b"
          />
        </v-col>
      </v-row>
      <v-row>
        <v-col class="btn-col"
          ><span style="font-size: 12px; text-align: left; color: #183ae0"
            >To prevent sandwich bots
          </span></v-col
        >
      </v-row>

      <!-- <v-row style="margin-top: 20px">
        <v-col class="btn-col">
          <v-btn color="#193BE3"
            ><v-img
              class="mr-3 inter-text"
              max-height="20px"
              max-width="20px"
              :src="require(`@/assets/info-icon.svg`)"
            /><span style="color: white; font-size: 15px"
              >How to buy $WGMI</span
            ></v-btn
          >
        </v-col>
      </v-row> -->
      <v-row class="my-12">
        <v-col class="btn-col">
          <v-img
            max-width="100px"
            style="margin: 0 auto"
            :src="require(`@/assets/wgmi-blue.png`)"
          />
        </v-col>
      </v-row>
      <v-row class="pt-12">
        <v-col class="btn-col inter-text" style="color: #193be3; font-size: 1rem;">
          Made with ♥️ for the $WGMI community. Design by
          <a href="https://twitter.com/h4nz013" target="_blank">h4nz013</a> and
          developped by
          <a href="https://twitter.com/0xMXCLL" target="_blank">MXKLL</a>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import CopyButton from "./CopyButton.vue";
import StoryButton from "./StoryButton.vue";
import { DISCORD_URL } from '@/config/constant.js'
export default {
  components: {
    StoryButton,
    CopyButton,
  },
  data: () => {
    return {
      DISCORD_URL: DISCORD_URL
    }
  }
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Rosaviro");
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@500&display=swap");

.story-container-1 {
  background-color: black;
  color: white;
  padding-bottom: 100px;
}

.story-container-2 {
  background-color: #193be2;
  color: white;
  padding-bottom: 50px;
}

.whole-container-3 {
  background-image: url("~@/assets/messages-art.png");
}

.story-container-3 {
  padding-top: 100px;
  background-size: cover;
}

.story-container-4 {
  padding-bottom: 100px;
}

.story-container-5 {
  background-color: #34fbeb;
}

.rosaviro {
  font-family: "Rosaviro";
}
.story {
  font-size: 5rem;

  text-align: center;
}

.description {
  font-size: 1rem;
  margin: 100px;
}

.img-container {
  width: 100%;
  z-index: 10;
  position: relative;
}

.img {
  position: relative;
  margin-top: -50px;
  z-index: 20;
}

.subtext {
  font-family: "Rosaviro";
  font-size: 2.5rem;
}

.community {
  font-family: "Rosaviro";
  font-size: 2rem;
  color: #f92a68;
  text-align: center;
  text-align: left;
}

.more-to-come {
  font-size: 2rem;
  font-family: "Rosaviro";

  color: #f92a68;
  text-align: center;
}

.btn-col {
  text-align: center;
}

.community-description-mobile {
  font-size: 1rem;
}

.community-description-text {
  background-color: rgb(52, 251, 235, 0.5);
}

.inter-text {
  font-family: "Inter", sans-serif;
}
</style>