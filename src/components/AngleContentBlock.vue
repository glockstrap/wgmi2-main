<template>
    <div class="angle-content-block-contain" :style="blockBackgroundCSS">
        <div class="angle-content-block">
            <div class="content-contain">
                <slot></slot>
            </div>
            <div :class="angleContainClasses" v-if="angle">
                <svg
                    class="angle"
                    width="100%"
                    viewBox="0 0 1514 235"
                    fill="none"
                    xmlns="http://www.w3.org/2000/svg"
                >
                    <path
                        d="M1514 0L-1 235L1514 70.708V0Z"
                        :fill="angleColor"
                    />
                </svg>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data: () => {
        return {
            reverse: false
        }
    },
    props: {
        angleColor: {
            type: String,
            default: "#FF0461",
        },
        bgColor: {
            type: String,
            default: "transparent",
        },
        angle: {
            type: Boolean,
            default: true
        }
    },
    computed: {
        angleBackgroundCSS() {
            return `background-color: ${this.angleColor};`;
        },
        blockBackgroundCSS() {
            return `background-color: ${this.bgColor};`;
        },
        angleContainClasses() {
            let classes = "angle-contain";
            if (this.angleReverse) {
                classes += " reverse";
            }
            return classes;
        },
    },
};
</script>

<style scoped>
.angle-contain {
    width: 100%;
}

.angle-contain.reverse {
    transform: scaleY(-1) scaleX(-1);
}

.angle {
    width: 100%;
}

.angle-content-block {
    transform: skewY(6.2deg);
}

.angle-content-block-contain {
    padding-bottom: 3.25%;
    margin-bottom: -9.5%;
    transform: skewY(-6.2deg);
    padding-top: 80px;
}

@media (max-width: 800px) {
    .angle-content-block-contain {
        padding-bottom: 2.25%;
    }
}
</style>