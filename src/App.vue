<template>
  <div>
    <ProductComponent
      v-if="product"
      :productType="product.type"
      :articleID="product.id"
      :imageURL="product.imageURL"
    />
    <p v-else>Loading...</p>
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";
import ProductComponent from "@/components/ProductC.vue";

const product = ref(null);

const fetchProductData = async () => {
  try {
    const response = await fetch(
      "https://full-api.onrender.com/api/product/get"
    );
    if (!response.ok) {
      throw new Error("Network response was not ok");
    }
    const result = await response.json();
    product.value = result[0];
  } catch (error) {
    console.error("Error fetching product data:", error);
  }
};

onMounted(() => {
  fetchProductData();
});
</script>