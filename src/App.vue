<template>
  <Navbar />
  <LandingPage1 />
  <LandingPage2 />
  <LandingPage3 />
  <LandingPage4 />
  <LandingPage5 />
  <LandingPage6 />
</template>

<script>
  import Navbar from "./components/navbar.vue"
  import LandingPage1 from "./components/LandingPage1.vue";
  import LandingPage2 from "./components/LandingPage2.vue";
  import LandingPage3 from "./components/LandingPage3.vue";
  import LandingPage4 from "./components/LandingPage4.vue";
  import LandingPage5 from "./components/LandingPage5.vue";
  import LandingPage6 from "./components/LandingPage6.vue";
  

  export default{
    components:{
      Navbar,
      LandingPage1,
      LandingPage2,
      LandingPage3,
      LandingPage4,
      LandingPage5,
      LandingPage6,
    }
  }
</script>

<style>

</style>