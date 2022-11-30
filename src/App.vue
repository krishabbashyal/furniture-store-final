<template>
  <div class="container">
    <Navbar/>
    <Shop/>
    <Grid/>
    <Footer/>
  </div>
</template>

<script>
import Navbar from './components/Navbar.vue'
import Shop from './components/Shop.vue'
import Grid from './components/Grid.vue';
import Footer from './components/Footer.vue';


export default {
  name: 'App',
  components: {
    Navbar,
    Shop,
    Grid,
    Footer,

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

.example {
  -ms-overflow-style: none;  /* IE and Edge */
  scrollbar-width: none;  /* Firefox */
}

.app {
  font-family: "Inter", sans-serif;
  overflow: hidden;
}

::-webkit-scrollbar {
    display: none;
}

</style>
