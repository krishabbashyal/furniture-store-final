<template>
    <div class="card">
        <img src="..\assets\beds\bed1.jpg" alt="">
        <h1>{{title}}</h1>
        <p>{{description}}</p>
        <p>${{price}}</p>
        <button>Add to cart</button>
 
    </div>
</template>

<script>
export default {
    name: 'Product',
    props: {
        title: {
            type: String
        },
        price: {
            type: String,
        },
        description: {
            type: String,
            default: "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut."
        }

    }
}
</script>

<style scoped>

.card {
    margin-top: 50px;
    margin-left: 101px;
    text-align: center;
    border: 1px solid black;
    width: 350px;
    height: 500px;
    border-radius: 15px;


}

img {
    width: 350px;
    border-top-left-radius: 15px;
    border-top-right-radius: 15px
    
}

</style>