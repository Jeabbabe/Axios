<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <div class="header">
    <h1 class="title">Forecast Web</h1>
    <div class="menu">
      <div>
        <RouterLink to="/">Home</RouterLink>
      </div>
      <div>
        <RouterLink to="/user">User</RouterLink>
      </div>
    </div>
  </div>
  <div><RouterView /></div>
</template>

<style scoped>
.header {
  display: grid;
  grid-template-columns: auto auto auto auto auto auto auto auto auto auto;
  margin-block: auto;
  padding: 30px;
  background: skyblue;
  font-size: 30px;
}
.menu {
  display: grid;
  grid-template-columns: auto auto;
  text-align: right;
  margin-block: auto;
}
.title {
  grid-column-start: 1;
  grid-column-end: 10;
}
</style>
