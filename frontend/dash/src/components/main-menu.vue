<script setup lang="ts">
import searchIcon from '../assets/searchicon.png'


</script>

<style scoped>
  body{
    margin: 0;
  }
  article{
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .header {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: row;
  }

  .header-left {
    color: var(--text);
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
    box-shadow: var(--box-shadow);
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

  .container {
    display: flex;
    flex-direction: row;
    justify-content: space-around;
    width: 80%;
    height: 35rem;


  }
  .watchlist, .detail {
    display: flex;
    justify-content: center;
    border-radius: 0.6rem;
    width: 40%;
    padding: 0 1rem;
    background-color: var(--bg);
    border-top: 2px solid var(--highlight);
    box-shadow: var(--box-shadow);
  }

</style>


<template>
  <body>
  <header>
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
  </header>
    <article>
      <div class="container">
        <div class="watchlist">
          <h1>Watchlist</h1>
        </div>
        <div class="detail">
          <h1>Details</h1>
        </div>
      </div>
    </article>
  </body>
</template>

