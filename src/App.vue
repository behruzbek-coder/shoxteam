<template>
  <div>
    <NavC />
    <filterComponent />
    <HeaderComponent />
    <ProductComponent />
    <SectionComponent /> 
    <FooterComponent />
  </div>
</template>

<script setup>
import NavC from './components/NavC.vue';
import filterComponent from './components/filterComponents.vue'
import ProductComponent from './components/ProductComponent.vue'
import HeaderComponent from './components/HeaderComponent.vue';
import SectionComponent from './components/SectionComponent.vue';
import FooterComponent from './components/FooterComponent.vue';
</script>

<style lang="scss" scoped>

</style>