<script setup lang="ts">


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
      <input class="search-input" type="text" placeholder="Search Stock" />
    </div>
  </div>
</div>
  </body>
</template>

