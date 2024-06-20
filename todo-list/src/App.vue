<script setup lang="ts">
import SearchableList from './components/SearchableList.vue'
</script>

<template>
  <main>
    <h2>Todo List</h2>
    <SearchableList  />
    
  </main>
</template>
<style>
ul {
    list-style-type: none;
}

button {
    border-radius: 5px;
    border: none;
    background-color: white;
    text-align: start;
    cursor: pointer
}
</style>