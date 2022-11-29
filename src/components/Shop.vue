<template>
    <div class="container">
        <div class="hero-section">
            <img src="..\assets\zHero\hero.jpg" alt="hero image">
            <h1>We design and build awesome furniture, for a better life.</h1>
            <p>In a small shop in the heart of our town, we spend our days relentlessly perfecting our products. The result is a perfect blend of beauty and comfort, that will have a lasting impact on your health without breaking the bank. </p>
            <div class="shop-by-section">
                <h2>Browse our inventory!</h2>
                <div class="button-span">
                  <Button text = "All"/>
                  <Button text = "Beds"/>
                  <Button text = "Chairs"/>
                  <Button text = "Couches"/>
                  <Button text = "Desks"/>
                  <Button text = "Dressers"/>
                  <Button text = "Tables"/>
                </div>

            </div>
        </div>


    </div>

</template>


<script>
    import Button from './Button.vue';
    export default {
      name: 'Shop',
      components: {
          Button,
          } 
      }


</script>


<style scoped>
.container{
    text-align: center;
    width: 60%;
    margin-bottom: 50px;
    
}
.hero-section{
    padding-top: 30px;
    font-size: 24px;
    letter-spacing: -1px;
    text-align: left;
    color: #343a40;  
    margin-left: 150px;  
}

.hero-section img{
    width: 500px;
    border-radius: 10%;
    float: right;
    margin-left: 50px;

}

.hero-section h1, h2{
    width: 50%;
}

.shop-by-section{
    margin-top: 30px;
    text-align: center;
    align-content: center;
    margin-bottom: 200px ;
}
.button-span{
    display: inline-flex
}


</style>