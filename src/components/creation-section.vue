<template>
    <section class="creation-section">
        <h1> Our creations</h1>
        <creation-card v-for="(creation,index) in creationData" :key="index" :creation="creation" />
        <div class="see-all">
            <button>see all</button>
        </div>
    </section>
</template>

<script>
import creationCard from './creation-card.vue';
import { reactive } from 'vue'

    export default{
        name:'creationSection',
        components:{
            creationCard,
        },

        setup(){
            const creationData=reactive({
                creation1:{
                    text:"Deep earth",
                    img:'images/mobile/image-deep-earth.jpg'
                },
                creation2:{
                    text:"Night arcade",
                    img:'images/mobile/image-night-arcade.jpg'
                },
                creation3:{
                    text:"Soccer team VR",
                    img:'images/mobile/image-soccer-team.jpg'
                },
                creation4:{
                    text:"The grid",
                    img:'images/mobile/image-grid.jpg'
                },
                creation5:{
                    text:"From up above VR",
                    img:'images/mobile/image-from-above.jpg'
                },
                creation6:{
                    text:"Pocket borealis",
                    img:'images/mobile/image-pocket-borealis.jpg'
                },
                creation7:{
                    text:"The curiosity",
                    img:'images/mobile/image-curiosity.jpg'
                },
                creation8:{
                    text:"Make it fisheye",
                    img:'images/mobile/image-fisheye.jpg'
                },
            });

            return{
                creationData
            }
        }
    }
</script>

<style>
    .creation-section{
        padding: 0px 8%;
        padding-bottom: 4rem;
    }
    .creation-section h1{
        margin-bottom: 35px;
        margin-top: 20px;
        text-align: center;
        font-family: 'Josefin Sans', sans-serif;
        text-transform: uppercase;
        font-size: 25px;
    }
    .see-all{
        margin-top: 30px;
        display: flex;
        justify-content: center;
    }
    .see-all button{
        background-color: transparent;
        border: 1px black solid;
        padding: 10px 35px;
        font-family: 'Josefin Sans', sans-serif;
        text-transform: uppercase;
    }
</style>