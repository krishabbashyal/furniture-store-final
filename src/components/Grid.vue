<template>
    <div class="shop-by-section">
                <h2>What are ya shoppin' for?</h2>
                <p>Select a category and we will show you all the hard work we have been up to</p>
                <div class="button-span">

                    <button class = "inactive" :class="{active: bedsButtonClicked }" @click="[beds = !beds, bedsButtonClicked = !bedsButtonClicked]">Beds</button>
                    <button class = "inactive" :class="{active: chairsButtonClicked }" @click="[chairs = !chairs, chairsButtonClicked = !chairsButtonClicked]">Chairs</button>
                    <button class = "inactive" :class="{active: couchesButtonClicked }" @click="[couches = !couches, couchesButtonClicked = !couchesButtonClicked]">Couches</button>
                    <button class = "inactive" :class="{active: dressersButtonClicked }" @click="[dressers = !dressers, dressersButtonClicked = !dressersButtonClicked]">Dressers</button>
                    <button class = "inactive" :class="{active: tablesButtonClicked }" @click="[tables = !tables, tablesButtonClicked = !tablesButtonClicked]">Tables</button>
                </div>
            </div>

    <div class="product-grid">
        <div v-if="beds" class="beds">
            <Product title = "The Luxury" price = "2499.99" image="bed1.jpg"/>
            <Product title = "The Rustic" price = "1599.99" image="bed3.jpg"/>
            <Product title = "The Modern" price = "1599.99" image="bed4.jpg"/>
            <Product title = "The Minimal" price = "1299.99" image="bed2.jpg"/>
            <Product title = "The Classic" price = "2299.99" image="bed5.jpg"/>
        </div>
        <div v-if="chairs" class="chairs">
            <Product title = "The Vintage" price = "199.99" image="chair2.jpg"/>
            <Product title = "The Eames" price = "799.99" image="chair4.jpg"/>
            <Product title = "The White Ice" price = "99.99" image="chair5.jpg"/>
            <Product title = "The Cloud" price = "99.99" image="chair3.jpg"/>
            <Product title = "The Mid-Century" price = "349.99" image="chair1.jpg"/>
        </div>
        <div v-if="couches" class="couches">
            <Product title = "The Abstract" price = "799.99" image="couch4.jpg"/>
            <Product title = "The Oval" price = "599.99" image="couch2.jpg"/>
            <Product title = "The Lonsdale" price = "799.99" image="couch3.jpg"/>
            <Product title = "The Reya" price = "599.99" image="couch5.jpg"/>
            <Product title = "The Midnight" price = "699.99" image="couch1.jpg"/>
        </div>
        <div v-if="dressers" class="dressers">
            <Product title = "The Oak" price = "399.99" image="dresser1.jpg"/>
            <Product title = "The Pearl" price = "399.99" image="dresser2.jpg"/>
            <Product title = "The Designer" price = "449.99" image="dresser3.jpg"/>
            <Product title = "The Oblong" price = "349.99" image="dresser4.jpg"/>
            <Product title = "The Southern" price = "599.99" image="dresser5.jpg"/>
        </div>
        <div v-if="tables" class="tables">
            <Product title = "The Mini" price = "499.99" image="table4.jpg"/>
            <Product title = "The Contemporary" price = "1099.99" image="table5.jpg"/>
            <Product title = "The Farmhouse" price = "299.99" image="table2.jpg"/>
            <Product title = "The Marble" price = "699.99" image="table3.jpg"/>
            <Product title = "The Laid Back" price = "399.99" image="table1.jpg"/>
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
        bedsButtonClicked: false,
        chairsButtonClicked: false,
        couchesButtonClicked: false,
        dressersButtonClicked: false,
        tablesButtonClicked: false,
	    beds: false,
        chairs: false,
        couches: false,
        desks: false,
        dressers: false,
        tables: false,
  	    }
    },
    methods: {
        myFilter: function() {
            this.isActive = !this.isActive;
            console.log("Changed the class")
        }
    }
}
    
</script>

<style scoped>

.product-grid{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
.shop-by-section{
    margin-top: 20px;
    margin-left: 200px;
    text-align: center;
    align-content: center;
    margin-bottom: 140px ;
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
.empty h1{
    font-size: 42px;
    color: rgba(128, 128, 128, 0.801);
}
.empty p{
    font-size: 24px;
    color: rgba(128, 128, 128, 0.801);
}
.inactive:hover {
    background-color: lightgreen;
}
.active:hover {
  background-color: red;

}
</style>