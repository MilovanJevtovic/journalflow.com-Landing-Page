<template>
    <main>
      <div v-if="showOverlay" class="overlay">
        <div class="modal">
          <button>Home</button>
          <button>Blog</button>
          <button>Pricing</button>
          <button>Support</button>
          <button>Login</button>
          <div>
            <button @click="showOverlay = false" class="close"><img src="./icons/delete-symbol-1-white.svg" alt=""></button>
          </div>
        </div>
      </div>
      <div class="wrap">
        <div class="icon-name">
          <img src="./icons/logo-white.png">
          <h1>JournalFlow</h1>
        </div>
        <div class="buttons">
          <button>Features</button>
          <button>Blog</button>
          <button>Pricing</button>
          <button>Support</button>
          <button>Login</button>
        </div>
        <button @click="showOverlay = true" class="hamburger"><img src="./icons/menu.svg"></button>
      </div>
    </main>
  </template>

  <script>

import {ref} from "vue"

const showOverlay = ref(false)

export default{
  name:'Navbar',
  data(){
    return{
      showOverlay: false,
    }
  }
}

</script>
  
  <style scoped>

  .hamburger{
    display: none;
  }

  main{
    background-color: #0B182B;
    height: 80px;
  }

  .wrap{
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 0px 12px;
    height: 80px;
    max-width: 960px;
    margin: 0 auto;
  }
  
  .icon-name{
    display: flex;
    align-items: center;
    cursor: pointer;
  }
  
  h1{
    font-size: 24px;
    color: white;
    font-weight: 500;
  }
  
   .buttons button{
    background-color: transparent;
    border: none;
    color: #9EA0A6;
    font-size: 16px;
    margin: 0px;
    margin-left: 30px;
    cursor: pointer;
    transition: color 0.15s, text-decoration 0.15s;
  }
  
  button:hover{
    color: white;
    text-decoration: underline;
  }
  
  
  .icon-name img{
    width: 32px;
    height: 32px;
    margin-right: 6px;
  }

  @media (max-width: 700px) {
    .buttons button{
      display: none;
    }

    .close{
      position: absolute;
      top: 15px;
      right: -175px;
    }

    .close img{
      width: 50px;
      height: 50px;
    }

    .hamburger{
      display: block;
      background: transparent;
      padding: 0px 0px;
      border: none;
      margin-right: 0px;
    }

    .hamburger img{
      height: 40px;
      width: 40px;
    }

    .overlay{
      position: absolute;
      z-index: 10;
      width: 100%;
      height: 100%;
      background-color: #0b182b;
      opacity: 0.95;
      padding-top: 80px;
      display: flex;
      justify-content: center;
    }
  
    .modal{
      display: flex;
      flex-direction: column;
    }

    .modal button{
      width: 100%;
      text-align: center;
      font-size: 24px;
      line-height: 60px;
      font-weight: 500;
      background-color: transparent;
      border: none;
      color: white;
    }
  
    .modal button:hover{
      text-decoration: underline;
    }

  }
  
  
  </style>