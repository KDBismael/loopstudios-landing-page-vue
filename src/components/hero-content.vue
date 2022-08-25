<template>
    <div class="hero-content">
        <p>{{content}}</p>
    </div>
</template>

<script>
    export default {
        name:'heroContent',
        props:{
            content:String,
        },
        setup(props){
            console.log(props.content)
        }
    }
</script>

<style scoped>
    .hero-content{
        border: 1.5px white solid;
        width: 100%;
        height: 180px;
        padding: 20px;
        display: grid;
        place-items: center;
    }
    .hero-content p{
        font-size: 34px;
        color: white;
        font-family: 'Josefin Sans', sans-serif;
        text-transform: uppercase;
        line-height: 35px;
    }
</style>