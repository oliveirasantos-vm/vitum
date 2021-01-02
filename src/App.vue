<template>
  <div id="app">
    <Navbar />
    <Main />
    <Biography />
  </div>
</template>

<script>
import Navbar from "./components/Navbar";
import Main from "./components/Main";
import Biography from "./components/Biography";
export default {
  name: "App",
  components: {
    Navbar,
    Main,
    Biography
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