<template>
    <main>
        <div class="wrap">
            <div class="buttons">
                <button>Terms of Service</button>
                <button>Privacy Policy</button>
                <button>FAQ</button>
                <button>Contact</button>
                <button>Changelog</button>
            </div>
            <div class="socials">
                <button><img src="./icons/twitter-grey.svg" alt=""></button>
                <button><img src="./icons/instagram-grey.svg" alt=""></button>
                <button><img src="./icons/facebook-grey.svg" alt=""></button>
                <button><img src="./icons/telegram-grey.svg" alt=""></button>
            </div>
        </div>
        <img class="logo" src="./icons/logo-white.png" alt="">
        <p>© 2020 JournalFlow. All rights reserved.</p>
    </main>
</template>

<script>
    export default {
        name:'Footer'
    }
</script>

<style scoped>

main{
    background-color: #0B182B;
    padding: 30px 0px;
    text-align: center;
}

.wrap{
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 960px;
    margin: 0 auto;
}

.buttons button{
    color: white;
    background-color: transparent;
    border: none;
    font-size: 15px;
    margin-right: 30px;
    color: #9EA0BA;
    cursor: pointer;
}

.buttons button:hover{
    text-decoration: underline;
}

.socials button{
    background-color: transparent;
    border: none;
    margin-left: 30px;
}

.socials img{
    height: 24px;
}
.logo{
    height: 60px;
    margin-top: 80px;
    margin-bottom: 20px;
}

p{
    color: #9EA0BA;
    font-size: 12px;
}

</style>