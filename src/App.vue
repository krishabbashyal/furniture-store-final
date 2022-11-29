<template>
  <div class="container">
    <Navbar/>
    <Shop/>
    <Grid/>

    



  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Shop from './components/Shop.vue'
import Grid from './components/Grid.vue';



export default {
  name: 'App',
  components: {
    Navbar,
    Shop,
    Grid,


  }
}
</script>










<style>

* {
margin: 0;
padding: 0;
background-color: #ffff;
color: #343a40;
}

.app {
  font-family: "Inter", sans-serif;
}


</style>
