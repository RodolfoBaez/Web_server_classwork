<script setup lang="ts">
//importing the router
import { RouterLink, RouterView } from 'vue-router'
//imoporting the defult hello world compnonet, lives within the components folder 
// vue turns markup language and adds programable ascepts such as varibles,. also allows for only sections 
// of an website to re-fresh when working. exmaple i change the navbar the body section does update. 
// you need to organize your code, view file(componet that gets brought by router), componet file(componet used in the app.vue)
</script>


<template>
  <header>
    <img alt="Vue logo" class="logo" src="@/assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      
      <nav>
        <RouterLink to="/">Home</RouterLink>
        <RouterLink to="/about">About</RouterLink>
      </nav>

    </div>
  </header>

  <RouterView />
  
</template>

<style scoped>

</style>
