<template>
    <main>
        <div class="wrap">
            <div class="left">
                <div class="top">
                    <h1>Keep a journal</h1>
                    <h1 style="color:#9EA0A6" class="secondh1">in your favourite messaging app.</h1>
                    <hr align="left">
                </div>
                <div class="bottom">
                    <h2>Try JournalFlow Free with</h2>
                    <div class="buttons">
                        <button><img src="./icons/telegram.png">Telegram</button>
                        <button><img src="./icons/messenger.svg">Facebook Messenger</button>
                        <button><img src="./icons/gmail.png">Email</button>
                    </div>
                    <p>Whatsapp, and Line and more app support is coming soon. <span>Get notified</span>.</p>
                </div>
            </div>
            <div class="right">
                <ul>
                    <li class="li1">Any amazing moment happen?</li>
                    <li class="li2">Which Friend do you miss most</li>
                    <li class="li3">What are you grateful for today?</li>
                    <li class="li4">typing...</li>
                </ul>
            </div>
        </div>
    </main>
</template>

<script>

    export default{
        name: 'LandingPage1'
    }

</script>

<style scoped>


    main{
        height: 720px;
        background-color: #0B182B;
    }

    .wrap{
        display: flex;
        justify-content: space-between;
        max-width: 960px;
        margin: 0 auto;
        position: relative;
    }

    h1{
        font-size: 36px;
        color: white;
        font-weight: 300;
    }

    h2{
        color: #9EA0A6;
        font-size: 20px;
        font-weight: 300;
    }

    hr{
        width: 60px;
        border: 4px solid #11ADB0;
    }

    .top{
        margin-top: 100px;
    }

    .bottom{
        margin-top: 180px;
    }

    img{
        height: 32px;
        padding-right: 10px;
    }

    .buttons{
        display: flex;
        flex-direction: row;
    }

    button{
        display: flex;
        flex-direction: row;
        align-items: center;
        padding: 10px 10px;
        margin-right: 20px;
        margin-top: 10px;
        margin-bottom: 10px;
        border-radius: 40px;
        font-size: 16px;
        font-weight: bold;
        background-color: rgba(52,142,255,.4);
        color: #348eff;
        cursor: pointer;
        border: none;
        transition: background-color 0.15s;
    }

    button:hover{
        background-color: rgba(52,142,255,.2);
    }

    p{
        margin-top: 30px;
        color: #9EA0A6;
        font-size: 10px;
    }

    span{
        color: #255cff;
        cursor: pointer;
        transition: text-decoration 0.15s;
    }

    span:hover{
        text-decoration: underline;
    }

    .right{
        width: 340px;
        height: 410px;
        position: absolute;
        top:100px;
        right: 0px;
    }

    .li1, .li2, .li3, .li4{
        color: white;
        list-style: none;
        padding: 20px 20px;
        font-weight: 100;
        opacity: 0;
        animation-name: slideInLeft;
        animation-duration: 1s;
        animation-fill-mode: forwards;
    }

    li:nth-child(1) {
        animation-delay: 1s;
   }
    li:nth-child(2) {
        animation-delay: 2s;
   }
    li:nth-child(3) {
        animation-delay: 3s;
   }
    li:nth-child(4) {
        animation-delay: 4s;
   }


    .li1{
        position: absolute;
        background-color: #A38EEE;
        border-radius: 30px 30px 0px 30px;
        top:0;
        right: 0;
    }

    .li2{
        position: absolute;
        background-color: #11ADB0;
        border-radius: 30px 30px 30px 0px;
        top:110px;
        left: 0px;
    }

    .li3{
        position: absolute;
        background-color: #1D2055;
        border-radius: 30px 30px 0px 30px;
        top: 220px;
        right: 0px;
    }

    .li4{
        position: absolute;
        background-color: #152F7D;
        border-radius: 30px 30px 30px 0px;
        top: 330px;
        right: 0px;
    }

    @keyframes slideInLeft {
        0%{opacity: 0; transform: translateY(100px);}
        100%{opacity: 1; transform: translateY(0px);}
    }


    @media (max-width: 700px) {
        
    ul{
        display: none;
    }
    .buttons{
        display: flex;
        flex-wrap: wrap;
    }
    button{
        justify-content: center;
    }

    .bottom p{
        display: none;
    }
    
    h1{
        font-size: 32px;
    }

    .secondh1{
        font-size: 22px;
    }

    hr{
        margin: 0px 0px;
    }

    .bottom{
        margin-top: 80px;
        margin-bottom: 20px;
    }

    main{
        height: auto;
        padding: 0px 12px;
    }

    .top{
        margin-top: 40px;
    }

    }
</style>