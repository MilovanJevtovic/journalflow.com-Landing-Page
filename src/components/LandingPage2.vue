<template>
    <main>
    <div class="wrap">
        <div class="up">
            <h1>✍️</h1>
            <h1 class="secondh1">Write from Anywhere</h1>
            <h2>Just like chatting with a friend</h2>
        </div>
        <div class="down">
            <div class="left">
                <div>
                    <h3>From Messaging Apps</h3>
                    <p>No new app needed. JournalFlow currently supports Telegram, Facebook Messenger, Email. Learn <span>how JournalFlow works</span>.</p>
                </div>
                <div>
                    <h3>On Any Platform</h3>
                    <p>Wanna journal on your iPhone / Android / Mac / PC? No problem. If your messaging app has an app on that platform, you can write a journal on that.</p>
                </div>
                <div>
                    <h3>Unleash the Power</h3>
                    <p>Don't limit by text. You can add photos, locations, moods in your journal. Audio and video support are coming soon.</p>
                </div>
            </div>
                <div class="right" id="right">
                    <img id="slide" :src="changeImg"  alt="">
                </div>
            </div>
    </div>
</main>
</template>

<script>

    let i = 0;
    let time = 3000;
        function changeImg(){
                let slide = ["src/components/images/screenshot-email.png", "src/components/images/screenshot-telegram.png", "src/components/images/screenshot-messenger.png"];
                document.getElementById('slide').src = slide[i];
                i = (i+1)%3;
        }
    setInterval(changeImg, time);
    window.onload = changeImg;

    export default {
        name:'LandingPage2',
        methods:{
            changeImg,
        }
    }

</script>

<style scoped>

    main{
        padding-bottom: 10px;
    }
    .wrap{
        max-width: 960px;
        margin: 0 auto;
    }

    .up{
        text-align: center;
    }

    img{
        width: 300px;
        border: 7px solid black;
        border-radius: 30px;
    }

    h1{
        font-size: 40px;
    }

    h2{
        font-size: 22px;
        color: #9EA0A6;
        margin: 20px 0px;
    }

    .down{
        display: flex;
        margin: 40px 0px;
    }

    .left{
        padding: 0px 120px;
    }

    .left div{
        margin: 40px 0px;
    }

    p{
        line-height: 25px;
        font-size: 15px;
    }

    span{
        color: blue;
        cursor: pointer;
    }

    span:hover{
        text-decoration: underline;
    }

    @media (max-width: 700px) {
        .down{
            display: flex;
            flex-direction: column;
            margin-top: 0px;
        }
        .right{
            text-align: center;
        }

        h1{
            font-size: 48px;
        }

        .secondh1{
            font-size: 24px;
        }

        h2{
            font-size: 16px;
            margin-bottom: 0px;
        }

        .left{
            padding: 20px 20px;
        }

      }



</style>