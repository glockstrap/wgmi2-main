<template>
    <div class="header-logo">
        <v-img :src="require(`@/assets/v2/logo_black_shadow1_1.png`)" alt="WGMI Logo" class="logo-image" />
    </div>
</template>

<script>
export default {
    methods: {
        scrollToTop() {
            window.scroll({
                top: 0,
                left: 0,
                behavior: "smooth",
            });
        },
    },
    mounted() {
        this.scrollToTop();
    },
};
</script>

<style scoped>
.logo-image {
    max-width: 700px;
    margin: 0 auto;
}
</style>