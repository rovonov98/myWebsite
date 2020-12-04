<template>
    <div class="preloader" v-if="!isLoaded">
        <div class="lds-ring"><div></div><div></div><div></div><div></div></div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            isLoaded: false
        }
    },
    mounted() {
        document.onreadystatechange = () => {
            if (document.readyState == "complete") {
                this.isLoaded = true;
            }
        }
    }
}
</script>

<style scoped lang="scss">
    .preloader {
        display: flex;
        justify-content: center;
        align-items: center;
        z-index: 3;
        width: 100vw;
        height: 100vh;
        background: $main-color-one;
    }
    .lds-ring {
        display: inline-block;
        position: relative;
        width: 80px;
        height: 80px;
    }
    .lds-ring div {
        box-sizing: border-box;
        display: block;
        position: absolute;
        width: 64px;
        height: 64px;
        margin: 8px;
        border: 8px solid $main-color-two;
        border-radius: 50%;
        animation: lds-ring 1.2s cubic-bezier(0.5, 0, 0.5, 1) infinite;
        border-color: $main-color-two transparent transparent transparent;
    }
    .lds-ring div:nth-child(1) {
        animation-delay: -0.45s;
    }
    .lds-ring div:nth-child(2) {
        animation-delay: -0.3s;
    }
    .lds-ring div:nth-child(3) {
        animation-delay: -0.15s;
    }
    @keyframes lds-ring {
    0% {
        transform: rotate(0deg);
    }
    100% {
        transform: rotate(360deg);
    }
    }

</style>