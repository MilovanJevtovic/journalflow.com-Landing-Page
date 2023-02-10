<template>
    <main>
      <div class="wrap">
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
      </div>
    </main>
  </template>
  
  <script>

  export default{
    name:'Navbar',
  }
  
  </script>
  
  <style scoped>
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
  
  button{
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
  
  
  img{
    width: 32px;
    height: 32px;
    margin-right: 6px;
  }

  @media (max-width: 700px) {
    button{
      display: none;
    }
  }
  
  
  </style>