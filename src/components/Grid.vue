<template>
    <div class="product-grid">
      <Product title = "Bed" price = "499.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "599.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "299.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "599.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "299.99" image="bed1.jpg"/>

      <Product title = "Bed" price = "299.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "499.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "499.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "599.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "299.99" image="bed1.jpg"/>

      <Product title = "Bed" price = "399.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "499.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "499.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "599.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "299.99" image="bed1.jpg"/>

      <Product title = "Bed" price = "499.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "599.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "299.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "599.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "299.99" image="bed1.jpg"/>

      <Product title = "Bed" price = "299.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "499.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "499.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "599.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "299.99" image="bed1.jpg"/>

      <Product title = "Bed" price = "399.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "499.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "499.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "599.99" image="bed1.jpg"/>
      <Product title = "Bed" price = "299.99" image="bed1.jpg"/>
    </div>
    
</template>

<script>
    import Product from './Product.vue';
    export default {
    name: 'Grid',
    components: {
        Product
        }
    }
</script>

<style>
.product-grid{
    display: flex;
    flex-wrap: wrap;
}
</style>