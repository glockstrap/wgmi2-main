<template>
    <v-btn :href="href" class="cta-button" color="#81F7EB" height="54px">
        <slot></slot>
    </v-btn>
</template>

<script>
export default {
    props: {
        href: {
            type: String,
            required: true
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
    font-size: 20px;
    text-transform: uppercase;
    letter-spacing: 0.07em;
    text-align: center;
    text-decoration: none;
}
</style>