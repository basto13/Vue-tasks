<template>
  <HelloWorld msg="Welcome to Your Vue.js App" />
  <ProductDetails />
</template>

<script>
import ProductDetails from "./components/ProductDetails.vue";

export default {
  name: "App",
  components: { ProductDetails },
};
</script>

<style></style>
