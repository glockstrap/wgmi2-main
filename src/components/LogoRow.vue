<template>
    <div class="logo-row">
        <div class="logo-circle-container">
            <v-img class="logo-circle" contain :src="require(`@/assets/v2/phoenix_crop.png`)" />
        </div>
        <div class="logo-circle-container">
            <v-img class="logo-circle" contain :src="require(`@/assets/v2/wgmi-vert_1.png`)" />
        </div>
        <div class="logo-circle-container">
            <v-img class="logo-circle" contain :src="require(`@/assets/v2/phoenix2_crop.png`)" />
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.logo-row {
    margin: 0px auto 60px;
    max-width: 1000px;
    display: flex;
    justify-content: center;
}

.logo-circle-container {
    padding: 20px;
    border-radius: 50px;
    border: 1px solid white;
    margin-right: 20px;
    margin-left: 20px;
}

.logo-circle {
    height: 50px;
    width: 50px;
}
</style>