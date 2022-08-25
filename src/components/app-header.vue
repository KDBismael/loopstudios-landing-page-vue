<template>
    <div class="header">
        <div class="logo">
            <img src="images/logo.svg" alt="logo">
        </div>
        <div class="menu">
            <img src="images/icon-hamburger.svg" alt="">
        </div>
        <div class="modal">
            <div class="overlay"></div>
            <div class="modal-content">
                <div class="head">
                    <div class="logo">
                        <img src="images/logo.svg" alt="logo">
                    </div>
                    <div class="close">
                        <img src="images/icon-close.svg" alt="">
                    </div>
                </div>
                <div class="option">
                    <span>About</span>
                    <span>Careers</span>
                    <span>Events</span>
                    <span>Products</span>
                    <span>Support</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default{
        name:'appHeader',
    }
</script>

<style scoped>
    .header{
        width: 100%;
        display: grid;
        grid-template-columns: repeat(2,minmax(auto,1fr));
        justify-items: end;
    }
    .logo{
        justify-self: start;
    }
    .logo img{
        width: 130px;
        height: auto;
        object-fit: cover;
        object-position: center;
    }
    .modal{
        position: fixed;
        z-index: 10;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background-color: black;
    }
    .modal .modal-content{
        padding: 29px 8%;
        color: white;
    }
    .modal .option {
        margin-top: 7rem;
        display: flex;
        flex-direction: column;
        row-gap: 15px;
    }
    .modal .option span{
        text-transform: uppercase;
        font-size: 20px;
        font-family: 'Josefin Sans', sans-serif;
    }
    .head{
        display: flex;
        justify-content: space-between;
    }
    .anime{
        transform: translateX(-100%);
        transition-property: transform;
        transition-duration: 1s;
        transition-timing-function: ease-in-out;
    }
</style>