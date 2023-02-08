<template>
  <link rel="stylesheet"  href="https://unpkg.com/xp.css">

<div id="outmost"  class="grid">

  <nav>
    <div class="window">
  <div class="title-bar">
    <div class="title-bar-text">Hello My Name Is...</div>
    <div class="title-bar-controls">
      <button aria-label="Minimize"></button>
      <button aria-label="Maximize"></button>
      <button aria-label="Close"></button>
    </div>

  </div>
  <!-- <div class="window-body"> -->
      <HomePage> 

      </HomePage>
  <!-- </div> -->
</div>
    
  </nav>

</div>
<router-view/>
</template>

<style>
*{
  margin: 0;
}
html { 
  background: url(./assets/Bliss.jpg) no-repeat center center fixed; 
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}
.grid{
  display: grid;
  place-items:center;
  transform: translate(0%, 5%);
}

</style>

<script>
import HomePage from './components/HomePage.vue';

export default {
  components: {
    HomePage
  }
}



</script>
