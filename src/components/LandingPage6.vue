<template>
    <div class="wrap">
        <div class="images">
            <img src="./icons/whatsapp-logo.png" alt="">
            <img src="./icons/line-logo.png" alt="">
            <img src="./icons/android-messages-logo.png" alt="">
            <img src="./icons/ios-messages.png" alt="">
        </div>
        <div>
            <h1>More messaging app support is coming soon.</h1>
            <h2>Subscribe for JournalFlow updates</h2>
        </div>
        <button>Subscribe</button>
    </div>
</template>

<script>
    export default {
        name:'LandingPage6',
    }
</script>

<style scoped>

.wrap{
    text-align: center;
}

.images{
    display: flex;
    justify-content: center;
    margin: 60px 0px;
}

img{
    width: 56px;
    margin: 0px 20px;
    animation-name: Appear;
    animation-duration: 5s;
    animation-iteration-count: infinite;
}

h1{
    font-size: 24px;
    font-weight: 300;
}

h2{
    font-size: 20px;
    font-weight: 500;
    color: #9EA0A6;
}

button{
    margin-top: 30px;
    margin-bottom: 50px;
    background-color: #F3F5F7;
    color: #255cff;
    padding: 0px 50px;
    border-radius: 30px;
    font-size: 16px;
    line-height: 50px;
    border: none;
    cursor: pointer;
}

button:hover{
    background-color: #EEEEEE;
    text-decoration: underline;
}

@keyframes Appear {
    0%{opacity: 0;}
    1%{opacity:1;}
}

</style>