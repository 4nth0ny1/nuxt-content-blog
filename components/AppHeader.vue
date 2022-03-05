<template>
  <header class="nav-container">
    <div class="title">
      <h2>Title</h2>
    </div>
    <div class="links">
      <NuxtLink class="nav-li" to="/">home</NuxtLink>
      <NuxtLink class="nav-li" to="/about">about</NuxtLink>
      <NuxtLink class="nav-li" to="/blog">blog</NuxtLink>
    </div>
  </header>
</template>

<script>
export default {
  name: "AppHeader"
};
</script>

<style>
  .nav-container {
    display: flex;  
    flex-direction: row;
    justify-content: space-between;
    border-bottom: 1px solid black;
    padding: 10px;
    align-items: center;
  }

  .nav-li {
    color: black;
    text-decoration: none;
    margin-left: 15px;
    margin-right: 15px;
  }


</style>