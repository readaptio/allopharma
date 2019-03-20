<template>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view/>  
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
body {
        margin: 0; padding: 0;
        font-family: 'Open Sans', Arial, sans-serif;
        box-sizing: border-box;
        background: linear-gradient(135deg, #41B883 0%,#354953 100%);
        background-size: cover;
        min-height: 100vh;
        color: #fff;
    }
    h1 {
        font-size: 6vw;
    }
    h1, h2, h3, h4 {
        margin: 0; padding: 0;
        font-family: 'Lobster', Arial, sans-serif;
    }
    .text-center {
        text-align: center;
    }
    .Wrap {
        max-width: 60vw;
        margin: 15vh auto;
    }
</style>
