<template>
    <section class="expertise-section">
        <div class="vr-image">
            <img src="images/mobile/image-interactive.jpg" alt="">
        </div>
        <div class="vr-content">
            <h1>The leader in interactive VR</h1>
            <p>Founded in 2011, Loopstudios has been producing world-class virtual reality projects for some of the best companies around the globe. Our award-winning creations have transformed businesses through digital experiences that bind to their brand.</p>
        </div>
    </section>
</template>

<script>
    export default{
        name:'expertiseSection',

    }
</script>

<style scoped>
    .expertise-section{
        padding: 60px 8%;
        padding-bottom:30px;
    }
    .vr-image img{
        width: 100%;
        height: auto;
        object-fit: cover;
        object-position: center;
    }
    .vr-content{
        padding: 30px;
        background-color: white;
        text-align: center;
    }
    .vr-content h1{
        margin-bottom: 15px;
        font-family: 'Josefin Sans', sans-serif;
        font-size: 25px;
        text-transform: uppercase;
    }
    .vr-content p{
        font-family: 'Alata', sans-serif;
        font-size: 12px;
        color: rgba(0, 0, 0, 0.6);
    }
</style>