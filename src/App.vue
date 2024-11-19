<script setup>
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <div class="wrapper">
    <nav class="menu">
      <RouterLink class="navButton" to="/">Home</RouterLink>
      <RouterLink class="navButton" to="/productos">Productos</RouterLink>
      <RouterLink class="navButton" to="/about">About</RouterLink>
      <RouterLink class="navButton" to="/contact">Contact</RouterLink>
    </nav>
  </div>

  <RouterView/>
</template>

<style scoped>
.wrapper{
  display: flex;
  height: 100%;
  width: 100%;
}
.menu{
  background-color: cyan;
  width: 100%;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  height: 75px;
}

.navButton{
  background-color: rgb(125, 125, 212);
  border-radius: 10px;
  color: rgb(255, 255, 255);
  width: 200px;
  height: 50px;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  transition: .5s;
}

.navButton:hover{
  background-color: rgb(83, 83, 187);

}

</style>
