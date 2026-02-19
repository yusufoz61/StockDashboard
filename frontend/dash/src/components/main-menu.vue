<script setup lang="ts">
import searchIcon from '../assets/searchicon.png'


</script>

<style scoped>
  body{
    margin: 0;
  }
  .header {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
  }

  .header-left {
    color: var(--text-color);
    font-weight: bold;
    font-size: 2rem;
    padding: 0 5rem;
  }


  .search {
    display: flex;
    align-items: center;
    justify-content: flex-end;
  }

  .search-input {
    width: 22rem;
    height: 2rem;
    outline: 2px solid var(--text-color);
    border: none;
    border-radius: 0.2rem;
    padding: 0.2rem 0.5rem;
  }

  .search-icon {
    width: 1.5rem;
    position: absolute;
    padding: 5px 5px;
    cursor: pointer;
  }

</style>


<template>
  <body>
<div class="header">
  <div class="header-left">
    <p>Stock Creeper</p>
  </div>
  <div class="header-right">
    <div class="search">
      <img :src="searchIcon" alt="search icon" class="search-icon" />
      <input class="search-input" type="text" placeholder="Search Stock" />
    </div>
  </div>
</div>
  </body>
</template>

