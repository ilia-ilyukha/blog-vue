<script setup lang="ts">
    import { RouterLink } from 'vue-router'
</script>
<template lang="">
    <header id="header">
      <h1><a href="#">Future Imperfect</a></h1>
      <nav class="links">
        <ul>
          <li><RouterLink to="/">Home</RouterLink></li>
          <li><RouterLink to="/test">Test</RouterLink></li>
          <li><a href="#">Feugiat</a></li>
          <li><a href="#">Tempus</a></li>
          <li><a href="#">Adipiscing</a></li>
        </ul>
      </nav>
      <nav class="main">
        <ul>
          <li class="search">
            <a class="fa-search" href="#search">Search</a>
            <form id="search" method="get" action="#">
              <input type="text" name="query" placeholder="Search" />
            </form>
          </li>
          <li class="menu">
            <a class="fa-bars" href="#menu">Menu</a>
          </li>
        </ul>
      </nav>
    </header>
</template>

<style lang="">
    
</style>