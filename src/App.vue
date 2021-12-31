<template>
    <v-app>
        <div class="app-main">
            <head-img />
            <logo-row />
            <intro-statement />

            <div class="button-group">
                <cta-button :contract="this.contractAddress">Copy Contract Address</cta-button>
                <cta-button href="https://app.mistx.io/#/exchange?outputCurrency=0x20f6a313cb250062331fe70b9567e3ee5f01888b">Buy on Mistx</cta-button>
                <div class="button-with-support">
                    <cta-button href="https://app.uniswap.org/#/swap?outputCurrency=0x20f6a313cb250062331fe70b9567e3ee5f01888b&slippage=2">Buy on Uniswap</cta-button>
                    <supporting-text
                        >2% slippage recommended for Uniswap</supporting-text
                    >
                </div>
                <div class="button-with-support">
                    <cta-button href="https://cowswap.exchange/#/swap?outputCurrency=0x20f6a313cb250062331fe70b9567e3ee5f01888b">Buy on Cowswap</cta-button>
                    <supporting-text>To prevent bot sandwiches</supporting-text>
                </div>
            </div>

            <retro-graphic></retro-graphic>

            <angle-content-block :angleColor="`#FF0461`" :bgcolor="`transparent`">
                <v-container class="angle-block-text">
                    <v-row align="center">
                        <v-col cols="12" md="6">
                            <v-layout align-center justify-center>
                                <div class="content-block-header">The<br>story</div>
                            </v-layout>
                        </v-col>
                        <v-col cols="12" md="6">
                            <p class="white--text">
                                of $WGMI began on November 11, 2021, during its launch. It started off as a promising memecoin that touched upon a popular saying in the crypto/NFT space, WGMI, which means <span style="color: #34fbeb">"We're Gonna Make It"</span>.                                
                            </p>
                            <p class="white--text">
                                However, the investors' enthusiasm soon turned sour when it was realized that the developer held a majority share and sold all of his stakes, bringing the price of $WGMI down to <span style="color: #f92a68">almost zero</span>.
                            </p>
                        </v-col>
                    </v-row>
                </v-container>
            </angle-content-block>

            <angle-content-block :angleColor="`transparent`" :bgColor="`#81F7EB`" :angleReverse="true">
                <v-container style="padding-top: 120px;" class="angle-block-text">
                    <v-row align="center">
                        <v-col cols="12" md="6">
                            <p class="black--text">
                                The victims, however, did not submit to this attack on honest participants of the space. The victims got together to form a community and decided to take over the coin, bringing the market cap from $80,000.00 to <span style="color: #FF0457">$30,000,000.00 within a day. </span>
                            </p>
                            <p class="black--text">
                                $WGMI is a story of how a small group of strong-headed individuals banded together to fight for what is right. All members of the community subscribe to the notion that, we will all truly make it.
                            </p>
                        </v-col>
                        <v-col cols="12"  md="6">
                            <v-layout align-center justify-center>
                                <div class="content-block-header">Community<br>Take Over</div>
                            </v-layout>
                        </v-col>
                    </v-row>
                </v-container>
            </angle-content-block>

            <angle-content-block :bgColor="`#ffffff`" :angleColor="`#FBE434`">
                <head-img class="contain-img" />
                <block-statement :color="`black`">represents hope and optimism for those who need it the most.</block-statement>
            </angle-content-block>

            <angle-content-block :bgColor="`#140033`" :angleColor="`transparent`" :angle="false">
                <v-container style="padding-top: 120px;" class="angle-block-text">
                    <v-row align="center">
                        <v-col cols="12" md="6">
                            <v-layout align-center justify-center>
                                <div class="content-block-header">Our Community.<br>Built Different.<br>From The Ashes.</div>
                            </v-layout>
                        </v-col>
                        <v-col cols="12" md="6">
                            <p class="white--text">
                                <span style="color: #81F7EB;">We're 100% community driven.</span><br>Rugger dev is gone and no longer owns any $WGMI or have ownership of the contract.
                            </p>

                            <p class="white--text">
                                This is for the People.<br>
                                This is for the Culture.
                            </p>
                        </v-col>
                    </v-row>

                    <v-img :src="require('@/assets/v2/community-messages_1.png')" class="community-img"></v-img>

                    <block-statement>And More to come...</block-statement>
                    
                    <v-row align="center" justify="center">
                        <v-col cols="6">
                            <cta-button href="https://discord.gg/wgmi" class="mt-6">Join Our Discord</cta-button>
                        </v-col>
                    </v-row>
                </v-container>
            </angle-content-block>

            <div class="angle-content-block-spacer"></div>
        </div>
    </v-app>
</template>

<script>
import HeadImg from "@/components/HeadImg.vue";
import LogoRow from "@/components/LogoRow.vue";
import IntroStatement from "@/components/IntroStatement.vue";
import CtaButton from "@/components/CTAButton.vue";
import SupportingText from "@/components/SupportingText.vue";
import RetroGraphic from "@/components/RetroGraphic.vue";
import AngleContentBlock from "@/components/AngleContentBlock.vue";
import BlockStatement from '@/components/BlockStatement.vue';

export default {
    name: "App",
    data: () => {
        return {
            contractAddress: '0x20f6a313cb250062331fe70b9567e3ee5f01888b'
        }
    },
    components: {
        HeadImg,
        LogoRow,
        IntroStatement,
        CtaButton,
        SupportingText,
        RetroGraphic,
        AngleContentBlock,
        BlockStatement
    }
};
</script>
<style>
html,
body,
.app-main {
    background-color: #1b072f;
}

.button-group {
    display: grid;
    max-width: 1000px;
    margin: 40px auto;
    grid-template-columns: 1fr 1fr;
    column-gap: 20px;
    row-gap: 20px;
    padding-right: 20px;
    padding-left: 20px;
}

@media (max-width: 800px) {
    .button-group {
        grid-template-columns: 1fr;
    }
}

.button-with-support {
    display: flex;
    flex-direction: column;
    row-gap: 20px;
}


.content-block-header {
    font-size: 60px;
    font-weight: bold;
    text-align: left;
    text-transform: uppercase;
    color: white;
    background: -webkit-linear-gradient(#ffc72a, #f51eb3);
    background-clip: text;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
}

.angle-block-text p {
    font-family: 'Lato', sans-serif;
    font-size: 18px;
    line-height: 1.8;
    padding-right: 24px;
    padding-left: 24px;
}

.contain-img {
    max-width: 600px;
    margin: 0 auto;
}

.community-img {
    margin-top: 80px;
    margin-bottom: 80px;
}

.angle-content-block-spacer {
    height: 300px;
    width: 100%;
    display: block;
    background-color: #140033;
}
</style>