<template>
    <div class="container">
        <div class="hero-section">
            <img src="..\assets\zHero\hero.jpg" alt="hero image">
            <h1>We design and build awesome furniture, for a better life.</h1>
            <p>In a small shop in the heart of our town, we spend our days relentlessly perfecting our products. The result is a perfect blend of beauty and comfort, that will have a lasting impact on your health without breaking the bank. </p>
            <div class="shop-by-section">
                <h2>Browse our inventory!</h2>
                <button>Beds</button>
                <button>Chairs</button>
                <button>Couches</button>
                <button>Desks</button>
                <button>Dressors</button>
                <button>Tables</button>
            </div>
        </div>


    </div>

</template>


<script>
export default {
    name: 'Shop'
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

button {
    margin-top: 5px;
    margin-left: 10px;
    background-color: white;;
    border-radius: 15px;
    padding: 10px;
    font-size: 22px;
    border: 2px solid black;

}

button:active{

}

button:hover{
    background-color: #00c97f;
}

</style>