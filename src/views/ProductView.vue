<script setup>
import productos from '@/assets/productos.json'
import { RouterLink, } from 'vue-router'

</script>

<template>
  <main>
    <div class="about">
      <h1>Product list</h1>
      <ul>
        <li v-for="product in productos" :key="product.id">
          <RouterLink :to="'productComponent/'+product.id">{{ product.name }}</RouterLink>
        </li>
      </ul>
    </div>
  </main>
</template>

<style scoped>
ul {
  width: auto;
  height: auto;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  justify-items: center;
  margin-top: 10px;
  padding: 0;
}

li {
  margin: 0;
  border: 1px dotted blue;
  margin: 5px;
  border-radius: 10px;
  background-color: rgb(229, 255, 0);
  list-style-type: none;
  width: 60%;
  height: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin:10px;
}
</style>
