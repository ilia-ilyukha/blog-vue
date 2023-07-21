<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue';
import Header from './components/common/Header.vue';
import Menu from './components/common/Menu.vue';
import Main from './components/common/Main.vue';
import Sidebar from './components/common/Sidebar.vue';

import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <!-- Wrapper -->
  <div id="wrapper">
    <!-- <RouterView /> -->
    <!-- Header -->
    <Header></Header>

    <!-- Menu -->
    <Menu></Menu>

    <!-- Main -->
    <Main></Main>

    <!-- Sidebar -->
    <Sidebar></Sidebar>

  </div>
</template>

<style scoped>
.logo {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  transition: filter 300ms;
}

.logo:hover {
  filter: drop-shadow(0 0 2em #646cffaa);
}

.logo.vue:hover {
  filter: drop-shadow(0 0 2em #42b883aa);
}</style>
