<template>
  <div id="sidebar">
    <nav>
      <router-link to="/domains">domains</router-link>
      <router-link to="/about">about</router-link>
      <router-link to="/">home</router-link>
    </nav>
  </div>
</template>

<style scoped lang="scss">
div#sidebar {
  margin: 0;
  padding: 1rem;
  min-height: 100vh;
  min-width: 35vw;
  background-color: #333;
}
</style>
