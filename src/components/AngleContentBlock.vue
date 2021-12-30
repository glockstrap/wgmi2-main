<template>
    <div class="angle-content-block">
        <div class="content-contain">
            <slot></slot>
        </div>
        <div class="angle-contain">
            <svg class="angle" height="235" viewBox="0 0 1440 235" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M1514 0L-1 235L1514 70.708V0Z" :fill="angleColor"/>
            </svg>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        angleColor: {
            type: String,
            default: '#FF0461'
        }
    },
    computed: {
        angleBackgroundCSS() {
            return `background-color: ${this.angleColor};`
        }
    }
}
</script>

<style scoped>
.angle-contain, .angle, .angle > path {
    width: 100%;
}

.angle-content-block {
    padding-bottom: 50px;
    margin-bottom: -50px;
}
</style>