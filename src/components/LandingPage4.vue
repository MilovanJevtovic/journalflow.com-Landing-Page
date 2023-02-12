<template>
    <main>
    <div class="wrap">
        <div class="up">
            <h1>⏳</h1>
            <h1 class="secondh1">Time Machine</h1>
            <h2>Bring back your best memories</h2>
        </div>
        <div class="down">
            <div class="left">
                <div>
                    <h3>Look back</h3>
                    <p>You can use our web app to view all your journals. It’s a fun way to remind yourself what happened in the past, and how far you’ve come.</p>
                </div>
                <div>
                    <h3>Smart reminder</h3>
                    <p>JournalFlow will remind you these memories in a smart way, like an anniversary.</p>
                </div>
            </div>
                <div class="right" id="right">
                    <img src="./images/screenshot-moments.png" alt="">
                </div>
            </div>
    </div>
</main>
</template>

<script>
    export default {
        name:'LandingPage4'
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