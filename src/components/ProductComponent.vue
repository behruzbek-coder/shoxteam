<template>
  <div class="main-product-container">
    <div v-for="product in products" :key="product.id" class="product-item">
      <div class="top-of-product">
        <div class="items">
          <p>Артикул: 515314</p>
          <h4>{{ product.name }}</h4>
        </div>

        <img class="heart-icon" src="../assets/images/Vector.svg" />
      </div>
      <img :src="product.url" class="product-image" alt="Product Image" />
      <div class="bottom-of-product">
        <h2>{{ product.name }}</h2>
        <div class="prices">
          <h1 class="seil">-{{ product.seil }}%</h1>
          <h1 class="oldPrice">{{ product.oldPrice }}</h1>
          <h1>{{ product.newPrice }}</h1>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";

const products = ref([]);
const loading = ref(true);
const error = ref(null);

const fetchProductData = async () => {
  loading.value = true;
  try {
    const response = await fetch(
      "https://full-api.onrender.com/api/product/get"
    );
    if (!response.ok) {
      throw new Error("Network response was not ok");
    }
    const result = await response.json();
    products.value = result.data;
  } catch (err) {
    error.value = err;
    console.error("Error fetching product data:", err);
  } finally {
    loading.value = false;
  }
};

onMounted(() => {
  fetchProductData();
});
</script>

<style scoped>
.product-item {
  margin-bottom: 20px;
  background: linear-gradient(
    180deg,
    rgba(0, 0, 0, 0.5) 0%,
    rgba(0, 0, 0, 0) 28.04%
  );
}

.prices {
  margin-top: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
}

.seil {
  background: #e24c55;
  color: #fff;
  padding: 2px 10px;
}

.oldPrice {
  text-decoration: line-through;
  text-decoration-color: red;
}

.prices {
  display: flex;
  gap: 10px;
}

h1 {
  font-size: 18px;
}

h2 {
  font-size: 14px;
}

p {
  font-size: 10px;
  color: white;
}

h4 {
  font-size: 12px;
  color: white;
}
.main-product-container {
  width: 230px;
  height: 240px;
  display: grid;
  gap: 24px;
  grid-template-columns: repeat(4, 1fr);
}

.product-image {
  width: 229px;
  height: 180px;
}

.items {
  display: flex;
  flex-direction: column;
}

.top-of-product {
  display: flex;
  justify-content: space-between;
  padding: 10px;
}

.bottom-of-product {
  text-align: center;
}
</style>
