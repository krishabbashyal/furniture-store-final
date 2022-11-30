<template>
    <div class="container">
        <div class="hero-section">
            <img src="..\assets\Hero\hero.jpg" alt="hero image">
            <h1>We design and build awesome furniture, for a better life.</h1>
            <p>In a small shop in the heart of our town, we spend our days relentlessly perfecting our products. The result is a perfect blend of beauty and comfort, that will have a lasting impact on your health without breaking the bank. </p>
            
        </div>
    </div>
</template>


<script>
    import Product from './Product.vue';
    export default {
      name: 'Shop',

      }


</script>


<style scoped>
.container{
    text-align: center;
    width: 75%;
    margin-bottom: 50px;
    
}
.hero-section{
    padding-top: 30px;
    font-size: 24px;
    letter-spacing: -1px;
    text-align: left;
    color: #343a40;  
    margin-left: 250px;


}

.hero-section img{
    width: 450px;
    border-radius: 10%;
    float: right;
    margin-left: 50px;

}



</style>