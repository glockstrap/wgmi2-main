<template>
    <div class="block-statement">
        <p :style="`${fontColorCSS};`"><slot></slot></p>
    </div>
</template>

<script>
export default {
    props: {
        color: {
            type: String,
            default: 'white'
        }
    },
    computed: {
        fontColorCSS() {
            return `color: ${this.color}`
        }
    }
}
</script>

<style scoped>
.block-statement {
    letter-spacing: 0.395em;
    font-weight: bold;
    text-transform: uppercase;
    max-width: 1000px;
    padding-right: 30px;
    padding-left: 30px;
    text-align: center;
    margin: 0 auto;
    font-size: 26px;

}
</style>