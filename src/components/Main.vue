<template>
  <div>
    <product-list :productlist="products" title="Våra sköna synthar" />
    <product-list :productlist="cart" title="Varukorg" />
  </div>
</template>

<script>
import ProductList from "./ProductList.vue";
export default {
  components: { ProductList },
  name: "Main",
  data() {
    return {
      products: [
        {
          productId: 30,
          name: "Volca FM",
          manufacturer: "Korg",
          price: 1199,
          imageUrl:
            "https://thumbs.static-thomann.de/thumb/thumb250x220/pics/prod/383318.jpg",
        },
        {
          productId: 3,
          name: "Volca Keys",
          manufacturer: "Korg",
          price: 1499,
          imageUrl:
            "https://thumbs.static-thomann.de/thumb/orig/pics/bdb/312865/8662697_800.webp",
        },
        {
          productId: 0,
          name: "PO-22",
          manufacturer: "Teenage Engineering",
          price: 799,
          imageUrl:
            "https://www.kjell.com/globalassets/productimages/729126_61909.tif?ref=8206E8072E&format=jpg&w=960&h=960&mode=pad",
        },
      ],
      cart: [
        {
          productId: 0,
          name: "PO-22",
          manufacturer: "Teenage Engineering",
          price: 799,
          imageUrl:
            "https://www.kjell.com/globalassets/productimages/729126_61909.tif?ref=8206E8072E&format=jpg&w=960&h=960&mode=pad",
        },
      ],
    };
  },
};
</script>

<style scoped>
div {
  width: 80%;
  margin: 0 auto;
  display: flex;
}
</style>
