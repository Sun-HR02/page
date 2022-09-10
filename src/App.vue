<template>
  <show-app></show-app>

</template>

<script>

import ShowApp from "@/components/show";
export default {
  name: 'App',
  components: {
    ShowApp,
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 3%;
}
body{
  background-color: black;
}

</style>
