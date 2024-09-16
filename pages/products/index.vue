<template>
  <div>
    <h1>Product List</h1>
    <div class="product-list">
      <ProductCard 
        v-for="product in products" 
        :key="product.id" 
        :product="product" 
      />
    </div>
  </div>
</template>

<script>
import ProductCard from '~/components/ProductCard.vue'; // Import the ProductCard component

export default {
  components: {
    ProductCard, // Register the component
  },
  data() {
    return {
      products: [
        { id: 1, name: "Product A", image: 'https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-01.jpg', shortDescription: "This is Product A" },
        { id: 2, name: "Product B", image: 'https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-02.jpg', shortDescription: "This is Product B" },
        { id: 3, name: "Product C", image: 'https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-03.jpg', shortDescription: "This is Product C" },
        { id: 4, name: "Product D", image: 'https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-04.jpg', shortDescription: "This is Product D" },
      ],
    };
  },
};
</script>

<style scoped>
.product-list {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}
</style>
