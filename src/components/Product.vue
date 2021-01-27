<template>
  <article>
    <h2>{{ Product.name }}</h2>
    <img :src="Product.imageUrl" />
    <p class="price">{{ Product.price }} SEK</p>
  </article>
</template>

<script>
export default {
  props: {
    Product: Object,
  },
};
</script>

<style scoped>
article {
  display: flex;
  text-align: left;
  padding: 0.33rem 1rem;
  border: thin solid silver;
  border-right: none;
  border-left: none;
}
h2 {
  flex: 60%;
}
p.price {
  flex: 20%;
}
img {
  flex: 20%;
  max-width: 100px;
  margin: 0 1rem;
}
</style>
