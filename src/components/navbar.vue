<template>
    <main>
      <div class="icon-name">
        <img src="./icons/logo-white.png">
        <h1>JournalFlow</h1>
      </div>
      <div>
        <button>Features</button>
        <button>Blog</button>
        <button>Pricing</button>
        <button>Support</button>
        <button>Login</button>
      </div>
    </main>
  </template>
  
  <script>

  export default{
    name:'Navbar',
  }
  
  </script>
  
  <style>
  main{
    background-color: #0B182B;
    display: flex;
    justify-content: space-around;
    align-items: center;
  }
  
  .icon-name{
    display: flex;
    align-items: center;
    cursor: pointer;
  }
  
  h1{
    font-size: 40px;
    color: white;
    font-weight: 100;
  }
  
  button{
    background-color: transparent;
    border: none;
    color: #9EA0A6;
    font-size: 20px;
    margin: 0px 15px;
    cursor: pointer;
    transition: color 0.15s, text-decoration 0.15s;
  }
  
  button:hover{
    color: white;
    text-decoration: underline;
  }
  
  
  img{
    width: 40px;
    height: 40px;
    margin-right: 6px;
  }
  
  
  </style>