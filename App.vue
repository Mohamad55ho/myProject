<template>

    <div id="app">
        <div class="auth-wrapper">
               <router-view />
        </div>
        <Footer/>
    </div>
</template>

<script>
        import Footer from './components/Footer.vue'

    export default {
        name: 'App',
        components: {
            Footer

        }
    }
    
</script>

<style>
    @import "https://cdn.jsdelivr.net/npm/animate.css@3.5.1";
    @import "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css";
    * {
        box-sizing: border-box;
    }

    body {
        background-image: url("https://images.pexels.com/photos/241044/pexels-photo-241044.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940");
        /*background: #1C8EF9 !important;*/
        background-position-x: 6%;
        background-position-y: 6%;
        min-height: 100vh;
        display: flex;
        font-weight: 400;
        font-family: 'Kaushan Script', cursive
    }

    h1, h2, h3, h4, h5, h6, label, span {
        font-weight: 500;
        font-family: 'Fira sana',sans-serif;
    }
    .element {
        top: 50%;
        left: 30%;
        padding-bottom:100px;
        margin-bottom:50px;
        text-align: center;
        line-height: 0px;
        border-width: 0;
        padding: 0;
        letter-spacing: 0px;
        font-weight: 400;
        font-size: 11px;
    }
    .footer {
        color: #020B4A;
        max-width:2000px;
        left: 10%;
        position: absolute;
        width: 20%;
        text-align: center
    }
    .nameLogo{
        display:inline-block;
    }
    /*h1 {
        font-family: Raleway;
        margin:0;
        padding: 0;
        text-align: center;
        position: absolute;
        top: 50%;
        left: 30%;
        transform: translate(-50%,-50%);
    }*/
    body, html, #app, #root, .auth-wrapper {
        width: 100%;
        height:60%;
    }

    #app {
        text-align: center;
    }
    .bg-img:after{
        position:absolute;
        content: '';
        top:0;
        left:0;
        height:100%;
        width:100%;
        background:rgba(0,0,0,0);
    }
    .content {
        position:absolute;
        top:50%;
        left:50%;
        transform:translate(-50%,-50%);
        text-align:center;
        z-index:999;
        padding:60px 32px;
        background: rgba(255,255,255,0.04);
        box-shadow: -1px 4px 28px 0px rgba(0,0,0,0.75)
        
        }
    
    .navbar-light {
        background-color: #ffffff;
        box-shadow: 0px 14px 80px rgba(34,35,58,0.2);
    }

    .auth-wrapper {
        display: flex;
        justify-content: center;
        flex-direction: column;
        text-align: left;
    }

    .auth-inner {
        width: 459px;
        margin: auto;
        background: #ffffff;
        box-shadow: 0px 14px 80px rgba(34,35,58,0.2);
        padding: 40px 55px 45px 55px;
        border-radius: 15px;
        transition: all .3s;
    }

    .auth-wrapper .form-control:focus {
        border-color: #167bff;
        box-shadow: none;
    }

    .auth-wrapper h3 {
        text-align: center;
        margin: 0;
        line-height: 1;
        padding-bottom: 20px;
    }

    .custom-control-label {
        font-weight: 400;
    }

    .forgot-password,
    .forgot-password a {
        text-align: right;
        font-size: 13px;
        padding-top: 10px;
        color: #7f7d7d;
        margin: 0;
    }

        .forgot-password a {
            color: #167bff;
        }
</style>
