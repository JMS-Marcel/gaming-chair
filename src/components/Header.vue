<script setup>
import { navData } from '@/data/data';
import { ref } from 'vue'

const navs = ref(navData);

</script> 

<template>
  <header id="home">
    <RouterLink to="/" class="logo">iChair</RouterLink>

    <ul class="nav">
      <li v-for="(nav) in navs" :key="nav.id
      ">
    <RouterLink to="/">{{ nav.name }}</RouterLink>  
    </li>
    </ul>
    <div class="features"></div>
    
  </header>
</template>

