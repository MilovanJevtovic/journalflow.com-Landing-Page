<template>
    <main>
    <div class="wrap">
        <div class="up">
            <h1>😆</h1>
            <h1 class="secondh1">Track Your Mood</h1>
            <h2>Express with an emoji</h2>
        </div>
        <div class="down">
            <div class="left">
                <div>
                    <h3>Remember the mood of the day</h3>
                    <p>It’s simple. Just send an emoji in chat or choose one on the web app. It also can be used to track weather, food, exercise, etc.</p>
                </div>
                <div>
                    <h3>Mood calendar</h3>
                    <p>All your moods will be organized into a calendar. It's easy to glance the trends of your life.</p>
                </div>
            </div>
                <div class="right" id="right">
                    <img src="./images/screenshot-mood.png" alt="">
                </div>
            </div>
    </div>
</main>
</template>

<script>
    export default {
        name:'LandingPage3'
    }
</script>

<style scoped>

    main{
        background-color: #F3F5F7;
        padding-bottom: 40px;
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
        border: 7px solid white;
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