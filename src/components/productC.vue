<template>
  <div class="my-product-component">
    <div class="top-of-product">
      <p>Артикул: {{ articleID }}</p>
      <p>{{ productType }}</p>
      <img src="@/assets/images/Vector.svg" />
    </div>
    <img :src="imageURL" alt="Product Image" />
  </div>
</template>
    
<script setup>
import { defineProps } from "vue";

const props = defineProps({
  productType: {
    type: String,
    default: "none",
  },
  articleID: {
    type: String,
    default: "none",
  },
  imageURL: {
    type: String,
    default: "none",
  },
});
</script>