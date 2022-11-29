<template>
    <div class="card">
        <img src="..\assets\beds\bed1.jpg" alt="">
        <h2>{{title}}</h2>
        <p class = "description">{{description}}</p>
        <p class = "price">${{price}}</p>
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
        },
    },

}
</script>

<style scoped>

.card {
 
    margin: 10px;
    margin-bottom: 20px;
    text-align: center;
    border: 1px solid black;
    width: 300px;
    height: 435px;
    border-radius: 15px;


}

img {
    width: 300px;
    border-top-left-radius: 15px;
    border-top-right-radius: 15px
}

button {
    margin-top: 0px;
    margin-left: 15px;
    background-color: white;;
    border-radius: 15px;
    padding: 8px;
    font-size: 14px;
    border: 2px solid black;
}

button:hover{
    background-color: #00c97f;
}

.price {
    font-weight: bold;
    margin: 8px;
    font-size: 18px;
}

.description{
    font-size: 14px;
}

</style>