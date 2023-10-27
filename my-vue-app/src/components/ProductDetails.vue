<template>
  <div>
    <h1>{{ product.name }}</h1>
    <p>Price: {{ formattedPrice }}</p>
    <p>{{ product.available ? "Available" : "Out of stock" }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      product: {
        name: "Sample Product",
        price: 99.99,
        available: true,
      },
    };
  },
  computed: {
    formattedPrice() {
      const price = this.product.price;
      return `$${price.toFixed(2)}`;
    },
  },
};
</script>

<style lang="scss" scoped></style>
