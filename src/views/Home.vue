<template>
  <div>
    <div class="home-hero"><home-hero></home-hero></div>
  </div>
</template>

<script>
  import HomeHero from '../components/HomeContent';


  export default {
    name: 'Home',
    components: { HomeHero }
  };
</script>

<style>
  .home-hero {
    background-image: url('../assets/cloud.png');
    background-position-x: 50%;
    background-position-y: 100%;
    background-repeat-y: no-repeat;
    background-repeat-x: repeat;
    width: 100%;
    height: 100%;
  }
</style>
