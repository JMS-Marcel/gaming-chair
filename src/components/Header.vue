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
<style scoped>
  header{
    position: relative;
    width: 95%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 30px 100px 30px 200px;
    z-index: 1100;
  }

  .logo{
    font-size: 35px;
    color: #fff;
    letter-spacing: 2px;
    font-weight: 800;
  }

  .nav{
    display: none;
  }

  .nav li{
    list-style: none;
    margin: 0 10px;
  }

  .nav li a{
    color: #fff !important;
    text-decoration: none;
    font-weight: 600;
    letter-spacing: 2px;
    cursor: pointer;
    transition: .3s;
  }

  .nav li:hover a,
  .nav li a.active{
    color: var(--primary);
  }
  .features{
    display: flex;
    align-items: center;
    gap:10px;
  }

  @media (max-width: 768px){
    header{
      padding: 10px 50px;
    }
    .nav{
      display: none;
    }
  }

</style>

