<template>
  <header>
    <nav>
      <ul>
        <li class="nav-item">
          <img class="logo" src="./assets/build-a-bot-logo.png" alt="logo" />
          Build-a-Bot
        </li>
      </ul>
    </nav>
  </header>
  <main>

    <!-- <HomePage msg="Welcome to Your Vue.js App" /> -->
    <RobotBuilder />
  </main>
</template>

<script setup>

import {ref, provide} from 'vue';
  //import HomePage from './Home/HomePage.vue';
  import RobotBuilder from './build/RobotBuilder.vue';
  //import ProductSearch from './ProductSearch.vue';

const userName = ref('Omega');
provide('userName', userName);
</script>

<style>
#app {
  font-family: Helvetica, Arial, sans-serif;
  
}


body{
    background: linear-gradient(to bottom, #555, #999);
    background-attachment: fixed;
}

</style>

<style scoped>

main{
  background: #fff; 
  margin: 0 auto;
  padding: 30px;
  width: 1400px;
  min-height: 300px;
}

header{
  background-color: #999;
  margin: 0 auto;
  width: 1460px;

}

ul {
 
  padding: 0;
  display: flex;
}
.nav-item {
  display: inline-block;
  padding: 5px 10px;
  font-size: 22px;
  border-right: 1px solid #bbb;
}
.logo{
  height: 30px;
  vertical-align: middle;
}
</style>
