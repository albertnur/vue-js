<template>
  <div id="app">
    <NavbarStarwars></NavbarStarwars>
    <FloatButton></FloatButton>
  </div>
</template>

<script>
import FloatButton from "./components/FloatButton";
import NavbarStarwars from "./components/NavbarStarwars";
export default {
  name: "App",
  components: {
    NavbarStarwars,
    FloatButton
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  height: 100vh;
  background: #ffffff;
  position: relative;
}
</style>
