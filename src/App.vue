<template>
  <link rel="stylesheet"  href="https://unpkg.com/xp.css">
<div id="outmost">
  <nav>
    <div class="window" style="width: 300px">
  <div class="title-bar">
    <div class="title-bar-text">A Window With Stuff In It</div>
    <div class="title-bar-controls">
      <button aria-label="Minimize"></button>
      <button aria-label="Maximize"></button>
      <button aria-label="Close"></button>
    </div>
  </div>
  <div class="window-body">
    <button>
      <router-link to="/">Home</router-link>
    </button>
    <button>
    <router-link to="/about">About</router-link>
    </button>
  </div>
</div>
    
  </nav>

  <p> Im Mr Tweet</p>
  <router-view/>
</div>
</template>

<style>
*{
  margin: 0;
}
#outmost{
  background-image: url("./assets/Bliss.jpg");
  background-repeat: no-repeat;
  width: 100%
}
</style>

<script>

</script>
