<template>
  <div class="my-product-component">
    <div class="top-of-product">
      <p>Артикул: {{ articleID }}</p>
      <p>{{ productType }}</p>
      <img src="@/assets/images/Vector.svg" />
    </div>
    <img :src="imageURL" />
    
  </div>
</template>
    
    <script>
export default {
  name: "ProductComponent",
  props: {
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

  },
};
</script>
    
<style scoped>
</style>
    