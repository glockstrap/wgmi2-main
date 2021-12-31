<template>
    <v-btn :href="hrefValue" class="cta-button" color="#81F7EB" height="54px" @click="copyContractAddress">
        <slot></slot>
    </v-btn>
</template>

<script>
export default {
    props: {
        href: {
            type: String,
            default: '#'
        },
        contract: {
            type: String,
            default: ''
        }
    },
    computed: {
        hrefValue() {
            if ( this.contract !== '' ) {
                return undefined
            }
            return this.href
        }
    },
    methods: {
        copyContractAddress(event) {
            if ( this.contract !== '' ) {
                const clipboardData =
                event.clipboardData ||
                window.clipboardData ||
                event.originalEvent?.clipboardData ||
                navigator.clipboard;

                clipboardData.writeText(this.contract);
            }
        }
    }
}
</script>

<style scoped>
.cta-button {
    background-color: #81F7EB;
    box-shadow: 7.84119px 8.82134px 10.7816px rgba(0, 0, 0, 0.25);
    color: black;
    width: 100%;
    border-radius: 4px;
    border: 1px solid #1B072F;
    font-weight: 600;
    
    text-transform: uppercase;
    letter-spacing: 0.07em;
    text-align: center;
    text-decoration: none;
    font-family: 'Lato', sans-serif;
}
</style>

<style>
.cta-button .v-btn__content {
    font-size: 20px;
}
</style>