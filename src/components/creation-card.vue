<template>
    <div>
        
    </div>
    <div :style="{backgroundImage:`url(${creation.img})`}" class="creation-card">
        <div class="overlay"></div>
        <span>{{creation.text}}</span>
    </div>
</template>

<script>
    export default {
        name:'creationCard',
        props:{
            creation:Object,
        },
        setup(){

        }
    }
</script>

<style scoped>
    .creation-card{
        position:  relative;
        background-repeat: no-repeat;
        background-position: center;
        background-size: cover;
        height: 90px;
        padding: 15px 15px;
        display: grid;
        align-items: end;
        justify-items:start ;
        color: white;
        margin: 15px 0px;
    }
    .creation-card span{
        font-family: 'Josefin Sans', sans-serif;
        text-transform: uppercase;
        font-size: 18px;
        width: 95px;
        z-index: 2;
    }
    .overlay{
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        background-color: rgba(0, 0, 0, 0.24);
    }
</style>