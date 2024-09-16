<template>
  <div>
    <h1 class="text-center m-8 text-2xl font-bold">
      HELPFUL TAGLINE / DESCRIPTION
    </h1>
    <div class="product-categories">
      <div class="product-list">
        <h2 class="uppercase text-center font-semibold">TRENDING: MEDICAL SUPPLIES</h2>
        <div class="flex flex-wrap justify-between">
          <ProductCard
            v-for="product in medical_products"
            :key="product.id"
            :product="product"
          />
        </div>
      </div>
      <div class="product-list">
        <h2 class="uppercase text-center font-semibold">TRENDING: AUTOMOTIVE</h2>
        <div class="flex flex-wrap justify-between">
          <ProductCard
            v-for="product in automotive_products"
            :key="product.id"
            :product="product"
          />
        </div>
      </div>
      <div class="product-list">
        <h2 class="uppercase text-center font-semibold">TRENDING: CONSUMER GOODS</h2>
        <div class="flex flex-wrap justify-between">
          <ProductCard
            v-for="product in consumer_products"
            :key="product.id"
            :product="product"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ProductCard from "~/components/ProductCard.vue"; // Import the ProductCard component

export default {
  components: {
    ProductCard, // Register the component
  },
  data() {
    return {
      medical_products: [
        {
          id: 1,
          name: "Product A",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-01.jpg",
          shortDescription: "This is Product A",
        },
        {
          id: 2,
          name: "Product B",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-02.jpg",
          shortDescription: "This is Product B",
        },
        {
          id: 3,
          name: "Product C",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-03.jpg",
          shortDescription: "This is Product C",
        },
        {
          id: 4,
          name: "Product D",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-04.jpg",
          shortDescription: "This is Product D",
        },
      ],
      automotive_products: [
        {
          id: 1,
          name: "Product A",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-05.jpg",
          shortDescription: "This is Product A",
        },
        {
          id: 2,
          name: "Product B",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-06.jpg",
          shortDescription: "This is Product B",
        },
        {
          id: 3,
          name: "Product C",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-07.jpg",
          shortDescription: "This is Product C",
        },
        {
          id: 4,
          name: "Product D",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-04-image-card-08.jpg",
          shortDescription: "This is Product D",
        },
      ],
      consumer_products: [
        {
          id: 1,
          name: "Product A",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-07-product-01.jpg",
          shortDescription: "This is Product A",
        },
        {
          id: 2,
          name: "Product B",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-07-product-02.jpg",
          shortDescription: "This is Product B",
        },
        {
          id: 3,
          name: "Product C",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-07-product-03.jpg",
          shortDescription: "This is Product C",
        },
        {
          id: 4,
          name: "Product D",
          image:
            "https://tailwindui.com/img/ecommerce-images/category-page-07-product-04.jpg",
          shortDescription: "This is Product D",
        },
      ],
    };
  },
};
</script>

<style scoped>
.product-list {
  background-color: white;
  padding: 15px;
  width: 450px;
}

.product-categories {
  display: flex;
  justify-content: space-between;
}
</style>
