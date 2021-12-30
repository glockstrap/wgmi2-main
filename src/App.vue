<template>
    <v-app>
        <div class="app-main">
            <head-img />
            <logo-row />
            <intro-statement />

            <div class="button-group">
                <cta-button href="#">Copy Contract Address</cta-button>
                <cta-button href="#">Buy on Mistx</cta-button>
                <div class="button-with-support">
                    <cta-button href="#">Buy on Uniswap</cta-button>
                    <supporting-text>2% slippage recommended for Uniswap</supporting-text>
                </div>
                <div class="button-with-support">
                    <cta-button href="#">Buy on Cowswap</cta-button>
                    <supporting-text>To prevent bot sandwiches</supporting-text>
                </div>
            </div>

            <retro-graphic></retro-graphic>

            <angle-content-block>
                <story />
            </angle-content-block>
            
        </div>
    </v-app>
</template>

<script>
import HeadImg from '@/components/HeadImg.vue'
import Story from '@/components/Story.vue'
import LogoRow from '@/components/LogoRow.vue'
import IntroStatement from '@/components/IntroStatement.vue';
import CtaButton from '@/components/CTAButton.vue';
import SupportingText from '@/components/SupportingText.vue';
import RetroGraphic from '@/components/RetroGraphic.vue';
import AngleContentBlock from '@/components/AngleContentBlock.vue';

export default {
    name: "App",
    components: {
        HeadImg,
        Story,
        LogoRow,
        IntroStatement,
        CtaButton,
        SupportingText,
        RetroGraphic,
        AngleContentBlock
    }
};
</script>
<style>
html,
body,
.app-main {
    overflow-x: hidden;
    background-color: #1B072F;
}

.button-group {
    display: grid;
    max-width: 1000px;
    margin: 40px auto;
    grid-template-columns: 1fr 1fr;
    column-gap: 20px;
    row-gap: 20px;
}

.button-with-support {
    display: flex;
    flex-direction: column;
    row-gap: 20px;
}
</style>