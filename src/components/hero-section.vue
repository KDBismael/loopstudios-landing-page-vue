<template>
    <section class="hero-section">
        <app-header/>
        <slot class="hero-content"></slot>
    </section>
</template>

<script>
import appHeader from './app-header.vue'


    export default{
        name:'heroSection',
        components:{
            appHeader
        },
        setup(){

        }
    }
</script>

<style scoped>
    .hero-section{
        padding: 25px 8%;
        background-image: url('images/mobile/image-hero.jpg');
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        height: 90vh;
        max-height: 490px;
        width: 100%;
        display: grid;
        grid-template-rows: auto 1fr;
        place-items: center;
    }
</style>