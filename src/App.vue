<template>
  <div id="app" style="width: 100%;
  height: 100%; 
  max-width: 700px; 
  display: flex;
  flex-direction: column;
  margin: 0 auto; 
  background: #ccc;">
    <Header />
    
    <router-view/>
  </div>
</template>

<script>

import Header from './components/layout/Header';

export default {
  name: 'app',
  components: {
    Header
  }
}
</script>

<style>
html, body {
  height: 100%;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
