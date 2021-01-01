<template>
  <div id="app">
    <Navbar />
    <Main />
  </div>
</template>

<script>
import Navbar from "./components/Navbar";
import Main from "./components/Main";
export default {
  name: "App",
  components: {
    Navbar,
    Main
  },
};
</script>

<style>
body {
  padding: 0;
  margin: 0;
  font-family: 'Work Sans', sans-serif;
  
}
</style>