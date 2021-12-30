<template>
  <div>
    <v-container class="story-container-1" fluid>
      <v-row>
        <v-col>
          <div class="story">The story</div>
        </v-col>
        <v-col>
          <div class="description inter-text">
            of $WGMI began on November 11, 2021, during its launch. It started
            off as a promising memecoin that touched upon a popular saying in
            the crypto/NFT space, WGMI, which means
            <span style="color: #34fbeb">"We're Gonna Make It"</span>. <br />
            <br />
            However, the investors' enthusiasm soon turned sour when it was
            realized that the developer held a majority share and sold all of
            his stakes, bringing the price of $WGMI down to
            <span style="color: #f92a68">almost zero</span>.
          </div>
        </v-col>
      </v-row>
    </v-container>
    <!-- <v-container class="story-container-2" fluid>
      <v-row>
        <v-col cols="6">
          <div class="description inter-text">
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
        </v-col>
        <v-col cols="6">
          <div class="img-container">
            <v-img
              class="img"
              :src="require(`@/assets/community-takeover-graphic.png`)"
            />
          </div>
        </v-col>
      </v-row>
      <v-container>
        <v-row style="margin-top: 100px">
          <v-col cols="1">
            <v-img
              max-width="100px"
              class
              :src="require(`@/assets/wgmi-vert.png`)"
            />
          </v-col>
          <v-col
            ><div class="subtext">
              represents hope and optimism for those who need it the most.
            </div></v-col
          >
        </v-row>
      </v-container>
    </v-container>
    <v-container class="story-container-3" fluid>
      <v-row>
        <v-col cols="4  " offset="1">
          <div class="community">
            Our community. <br />
            Built different. <br />
            From the ashes.
          </div>
        </v-col>
        <v-col>
          <div class="community-description inter-text">
            We’re 10<span class="community-description-text pr-10 pt-2"
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
        </v-col>
      </v-row>
      <div class="pa-10">
        <v-img :src="require(`@/assets/community-messages.png`)" />
      </div>
    </v-container>
    <v-container class="story-container-4">
      <v-row>
        <v-col>
          <div class="more-to-come">And more to come...</div>
        </v-col>
      </v-row>
      <v-row>
        <v-col class="join-discord">
          <story-button
            text="JOIN OUR DISCORD"
            hreflink="https://discord.gg/ReWXytCD"
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
    <v-container fluid class="story-container-5">
      <v-row>
        <v-col>
          <div class="img-container">
            <v-img
              class="img"
              :src="require(`@/assets/join-movement-graphic.svg`)"
            />
          </div>
        </v-col>
        <v-col style="margin-left: 100px">
          <v-row style="margin-top: 200px">
            <copy-button
              text="COPY CONTRACT ADDRESS"
            />
          </v-row>
          <v-row style="margin-top: 30px">
            <story-button
              text="BUY ON UNISWAP"
              hreflink="https://app.uniswap.org/#/swap?outputCurrency=0x20f6a313cb250062331fe70b9567e3ee5f01888b&slippage=2"
            />
          </v-row>
          <v-row
            class="inter-text"
            style="
              margin-top: 30px;
              font-size: 16px;
              color: #183ae0;
              font-weight: 500;
            "
          >
            <v-img
              class="mr-3"
              max-height="20px"
              max-width="20px"
              :src="require(`@/assets/attention-icon.svg`)"
            />2% slippage recommended for Uniswap
          </v-row>
          <v-row style="margin-top: 100px">
            <story-button
              text="BUY ON MISTX"
              hreflink="https://app.mistx.io/#/exchange?outputCurrency=0x20f6a313cb250062331fe70b9567e3ee5f01888b"
            />
          </v-row>
          <v-row style="margin-top: 30px">
            <story-button
              text="BUY ON COWSWAP"
              hreflink="https://cowswap.exchange/#/swap?outputCurrency=0x20f6a313cb250062331fe70b9567e3ee5f01888b"
            />
          </v-row>
          <v-row
            class="inter-text"
            style="
              margin-top: 30px;
              font-size: 16px;
              color: #183ae0;
              font-weight: 500;
            "
          >
            To prevent bot sandwiches
          </v-row>

          <v-row style="margin-top: 100px">
            <v-btn color="#193BE3" x-large class="story-btn"
              ><v-img
                class="mr-3 inter-text"
                max-height="20px"
                max-width="20px"
                :src="require(`@/assets/info-icon.svg`)"
              /><span style="color: white"
                >Here’s a guide on how to buy $WGMI</span
              ></v-btn
            >
          </v-row>
        </v-col>
      </v-row>
      <v-row class="pt-12">
        <v-col class="join-discord inter-text" style="color: #193be3;">
          Made with ♥️ for the $WGMI community. Design by <a href="https://twitter.com/h4nz013" target="_blank">h4nz013</a> and developped by <a href="https://twitter.com/0xMXCLL" target="_blank">MXKLL</a>
        </v-col>
      </v-row>
    </v-container> -->
  </div>
</template>

<script>
// import CopyButton from './CopyButton.vue';
// import StoryButton from "./StoryButton.vue";
export default {
  components: {
    // StoryButton,
    // CopyButton,
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css?family=Rosaviro");
@import url("https://fonts.googleapis.com/css2?family=Inter:wght@500&display=swap");

.story-container-1 {
  color: white;
  padding-bottom: 200px;
  padding-left: 120px;
  padding-right: 120px;
}

.story-container-2 {
  background-color: #193be2;
  color: white;
  padding-bottom: 200px;
  padding-top: 100px;
  padding-left: 120px;
  padding-right: 120px;
}

.story-container-3 {
  padding-top: 100px;
  background-image: url("~@/assets/messages-art.png");
  background-size: cover;
  padding-left: 120px;
  padding-right: 120px;
}

.story-container-4 {
  padding-bottom: 300px;
  padding-left: 120px;
  padding-right: 120px;
}

.story-container-5 {
  background-color: #34fbeb;
  padding-left: 120px;
  padding-right: 120px;
  padding-bottom: 100px;
}

.story {
  font-size: 5rem;
  font-family: "Rosaviro";
  text-align: center;
}

.description {
  font-size: 1rem;
}

.img-container {
  z-index: 10;
  position: relative;
}

.img {
  position: relative;
  margin-top: -200px;
  z-index: 20;
}

.subtext {
  font-family: "Rosaviro";
  font-size: 2.5rem;
}

.community {
  font-family: "Rosaviro";
  font-size: 3rem;
  color: #f92a68;
  text-align: center;
  text-align: left;
}

.more-to-come {
  font-size: 4rem;
  font-family: "Rosaviro";

  color: #f92a68;
  text-align: center;
}

.join-discord {
  text-align: center;
}

.community-description {
  font-size: 1.5rem;
  padding-left: 20%;
  text-align: left;
}

.community-description-text {
  background-color: rgb(52, 251, 235, 0.5);
}

.inter-text {
  font-family: "Inter", sans-serif;
}
</style>