<template>
  <div id="app">
    <app-navigation></app-navigation>
    <router-view/>
  </div>
</template>
<style>
  @import url("https://fonts.googleapis.com/css2?family=Baloo+Tamma+2:wght@500&display=swap");
  * {
    font-family: "Baloo Tamma 2", cursive;
  }
  body {
    text-align: center;
    padding: 0px;
    margin: 0px;
    background-color: rgb(52, 73, 94);
  }
</style>
<script>
  import AppNavigation from "./components/AppNavigation";
  export default {
    components: {AppNavigation}
  }
</script>