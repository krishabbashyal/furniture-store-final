<template v-if="">
    <div class="shop-by-section">
                <h2>What are ya shoppin' for?</h2>
                <p>Select a category and we will show you all the hard work we have been up to 😏😏</p>
                <div class="button-span">

                    <button @click="beds = !beds">Beds</button>
                    <button @click="chairs = !chairs">Chairs</button>
                    <button @click="couches = !couches">Couches</button>
                    <button @click="desks = !desks">Desks</button>
                    <button @click="dressers = !dressers">Dressers</button>
                    <button @click="tables = !tables">Tables</button>    
                </div>
            </div>

    <div class="product-grid">
        <div v-if="beds" class="beds">
            <Product title = "beds" price = "499.99" image="bed1.jpg"/>
            <Product title = "beds" price = "599.99" image="bed1.jpg"/>
            <Product title = "beds" price = "299.99" image="bed1.jpg"/>
            <Product title = "beds" price = "599.99" image="bed1.jpg"/>
            <Product title = "beds" price = "599.99" image="bed1.jpg"/>
        </div>
        <div v-if="chairs" class="chairs">
            <Product title = "chairs" price = "499.99" image="bed1.jpg"/>
            <Product title = "chairs" price = "599.99" image="bed1.jpg"/>
            <Product title = "chairs" price = "299.99" image="bed1.jpg"/>
            <Product title = "chairs" price = "599.99" image="bed1.jpg"/>
            <Product title = "chairs" price = "599.99" image="bed1.jpg"/>
        </div>
        <div v-if="couches" class="couches">
            <Product title = "couchs" price = "499.99" image="bed1.jpg"/>
            <Product title = "couchs" price = "599.99" image="bed1.jpg"/>
            <Product title = "couchs" price = "299.99" image="bed1.jpg"/>
            <Product title = "couchs" price = "599.99" image="bed1.jpg"/>
            <Product title = "couchs" price = "599.99" image="bed1.jpg"/>
        </div>
        <div v-if="desks" class="desks">
            <Product title = "desks" price = "499.99" image="bed1.jpg"/>
            <Product title = "desks" price = "599.99" image="bed1.jpg"/>
            <Product title = "desks" price = "299.99" image="bed1.jpg"/>
            <Product title = "desks" price = "599.99" image="bed1.jpg"/>
            <Product title = "desks" price = "599.99" image="bed1.jpg"/>
        </div>
        <div v-if="dressers" class="dressers">
            <Product title = "dressers" price = "499.99" image="bed1.jpg"/>
            <Product title = "dressers" price = "599.99" image="bed1.jpg"/>
            <Product title = "dressers" price = "299.99" image="bed1.jpg"/>
            <Product title = "dressers" price = "599.99" image="bed1.jpg"/>
            <Product title = "dressers" price = "599.99" image="bed1.jpg"/>
        </div>
        <div v-if="tables" class="tables">
            <Product title = "tables" price = "499.99" image="bed1.jpg"/>
            <Product title = "tables" price = "599.99" image="bed1.jpg"/>
            <Product title = "tables" price = "299.99" image="bed1.jpg"/>
            <Product title = "tables" price = "599.99" image="bed1.jpg"/>
            <Product title = "tables" price = "599.99" image="bed1.jpg"/>
        </div>
    </div>
</template>

<script>
    import Product from './Product.vue';
    export default {
    name: 'Grid',
    components: {
        Product
    },
    data() {
  	    return {
	    beds: false,
        chairs: false,
        couches: false,
        desks: false,
        dressers: false,
        tables: false
  	}
}
    }
    
</script>

<style>
.product-grid{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

.shop-by-section{
    margin-top: 50px;
    margin-left: 200px;
    text-align: center;
    align-content: center;
    margin-bottom: 200px ;
}
.button-span{
    display: inline-flex
}

.beds{
    display: flex;
}

.chairs{
    display: flex;
}
.couches{
    display: flex;
}
.desks{
    display: flex;
}
.dressers{
    display: flex;
}
.tables{
    display: flex;
}

button {
    margin-top: 5px;
    margin-left: 15px;
    background-color: white;;
    border-radius: 15px;
    padding: 10px;
    font-size: 22px;
    border: 2px solid black;
}
.active{
    background-color: #005838;
    color: white;

}
button:hover{
    background-color: #00c97f;
}

.empty h1{
    font-size: 42px;
    color: rgba(128, 128, 128, 0.801);
}

.empty p{
    font-size: 24px;
    color: rgba(128, 128, 128, 0.801);
}



</style>