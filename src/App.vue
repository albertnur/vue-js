<template>
  <div id="app">
    <NavbarStarwars></NavbarStarwars>
    <float-button @characters-added="showCharacters"></float-button>
    <div class="container">
      <CharacterList :characters="characters"></CharacterList>
    </div>
  </div>
</template>

<script>
import NavbarStarwars from "./components/NavbarStarwars";
import FloatButton from "./components/FloatButton";
import CharacterList from "./components/CharacterList";

export default {
  name: "App",
  components: {
    NavbarStarwars,
    FloatButton,
    CharacterList
  },

  data(){
    return{
      characters:[]
    }
  },
  
  methods: {
    showCharacters(payload) {
      this.characters = payload;
      console.log(payload);
    }
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100vh;
  position: relative;
}
</style>
