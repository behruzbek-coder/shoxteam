<template>
  <div>
    <h1>Processed Data from API:</h1>
    <ul v-if="processedData.length">
      <li v-for="item in processedData" :key="item.id">
        {{ item.displayName }}
      </li>
    </ul>
    <p v-else>No data available</p>
    <p v-if="loading">Loading...</p>
    <p v-if="error">{{ error.message }}</p>
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";

let data = [];
const processedData = ref([]);
const loading = ref(true);
const error = ref(null);

const processData = () => {
  console.log(data)
  data.value.forEach(element => {
    console.log(element.name)
  });
};

const fetchData = async () => {
  loading.value = true;
  try {
    const response = await fetch(
      "https://full-api.onrender.com/api/product/get"
    );
    if (!response.ok) {
      throw new Error("Error");
    }
    const result = await response.json();
    console.log(result);
    data.value = result.data;
    processData();
  } catch (err) {
    error.value = err;
    console.error("Error:", err);
  } finally {
    loading.value = false;
  }
};

onMounted(() => {
  fetchData();
});
</script>
