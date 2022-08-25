<template>
    <div class="footer">
        <div>
            <div class="logo">
                <img src="/images/logo.svg" alt="">
            </div>
            <div class="option">
                <span>About</span>
                <span>Careers</span>
                <span>Events</span>
                <span>Products</span>
                <span>Support</span>
            </div>
        </div>
        <div>
            <div class="social">
                <div class="fb">
                    <img src="/images/icon-facebook.svg" alt="">
                </div>
                <div class="tw">
                    <img src="/images/icon-twitter.svg" alt="">
                </div>
                <div class="pin">
                    <img src="/images/icon-pinterest.svg" alt="">
                </div>
                <div class="ig">
                    <img src="/images/icon-instagram.svg" alt="">
                </div>
            </div>
            <p>© 2021 Loopstudios. All rights reserved</p>
        </div>
    </div>
</template>

<script>
    export default{
        name:'appFooter',

    }
</script>

<style scoped>
    .footer{
        padding: 60px 8%;
        background-color: black;
        color: white;
    }
    p{
        text-align: center;
        margin-top: 15px;
        font-size: 12px;
    }
    .logo{
        display: flex;
        justify-content: center;
        margin-bottom: 30px;
    }
    .logo img{
        width: 130px;
        height: auto;
        object-fit: cover;
        object-position: center;
    }
    .option{
        display: flex;
        flex-direction: column;
        align-items: center;
        row-gap: 15px;
    }
    .option span{
        font-size: 13px;
    }
    .social{
        display: flex;
        justify-content: center;
        column-gap: 15px;
        margin-top: 30px;
    }
</style>