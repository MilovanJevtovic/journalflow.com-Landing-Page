<template>
    <main>
    <div class="wrap">
        <div class="up">
            <h1 style="font-size: 65px;">📱</h1>
            <h1>Manage in One Place</h1>
            <h2>on journalflow.com</h2>
        </div>
        <div class="down">
            <div class="left">
                <div>
                    <h3>Manage journals</h3>
                    <p>You can list / view / edit / delete journals on journalflow.com.</p>
                </div>
                <div>
                    <h3>Write different day entry</h3>
                    <p>If someday's journal is forgotten, don't worry. You can fix it on journalflow.com</p>
                </div>
                <div>
                    <h3>Analytics</h3>
                    <p>The statistic about your journal will help you know yourself better, even build new habits.</p>
                </div>
            </div>
                <div class="right" id="right">
                    <img src="./images/screenshot-account.png" alt="">
                </div>
            </div>
    </div>
</main>
</template>

<script>
    export default {
        name:'LandingPage5'
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
        }
        .right{
            text-align: center;
        }
      }

</style>