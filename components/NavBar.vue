<template>
  <header>
    <nuxt-link to="/" class="brand">Home</nuxt-link>
    <nav>
      <nuxt-link to="/articles">Article List</nuxt-link>&nbsp;|
      <nuxt-link to="/about">About</nuxt-link>
    </nav>
  </header>
</template>

<style scoped>
.brand {
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  font-size: 1.5em;
  color: red;
  text-decoration: none;
}
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 60px;
}
header .nav-item {
  box-sizing: border-box;
  margin: 0 5px;
  color: rgba(0, 0, 0, 0.5);
  text-decoration: none;
}
header .nav-item.router-link-exact-active {
  color: red;
  border-bottom: solid 2px red;
}
header a {
  display: inline-block;
}
</style>
