<template>
  <div class="app">
    <!-- <div id="nav">
      <router-link to="/">Home</router-link> |
      <router-link to="/about">About</router-link>
    </div> -->
    <router-view />
  </div>
</template>

<style>
:root {
  background-color: rgb(112, 110, 105);
  font-size: 2em;
}

.app {
  width: 100vw;
  height: 100vh;
  overflow-y: scroll;
  scrollbar-width: none;
}

.app::-webkit-scrollbar {
  display: none;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
