<template>
  <section>
    <h1>{{ title }}</h1>
    <Product v-for="product in productlist" :Product="product" :key="product.id" />
  </section>
</template>

<script>
import Product from "./Product.vue";
export default {
  name: "ProductList",
  components: {
    Product,
  },
  props: {
    productlist: Array,
    title: String,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Bodoni+Moda&display=swap");
h1,
h2,
p {
  font-family: "Bodoni Moda", serif;
}
section {
  flex: 0 1 auto;
  margin: 0 1rem;
}
</style>
