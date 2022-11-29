<template>
    <div class="container">
        <button>{{text}}</button>
    </div>
</template>

<script>
    export default {
    name: 'Button',
    props: {
        text: String,
    },

    }
</script>

<style >
.product-grid{
    display: flex;
    flex-wrap: wrap;
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

button:active{

}

button:hover{
    background-color: #00c97f;
}
</style>