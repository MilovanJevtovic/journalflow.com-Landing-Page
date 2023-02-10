<template>
  <Navbar />
  <LandingPage1 />
  <LandingPage2 />
</template>

<script>
  import Navbar from "./components/navbar.vue"
  import LandingPage1 from "./components/LandingPage1.vue";
  import LandingPage2 from "./components/LandingPage2.vue";
  

  export default{
    components:{
      Navbar,
      LandingPage1,
      LandingPage2,
    }
  }
</script>

<style>

</style>