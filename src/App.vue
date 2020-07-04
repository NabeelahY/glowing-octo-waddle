<template>
  <div id="app">
    <Navbar />
    <Hero />
    <About />
    <Services />
    <Team />
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Hero from "./components/Hero.vue";
import About from "./components/About.vue";
import Services from "./components/Services.vue";
import Team from "./components/Team.vue";


export default {
  name: "App",
  components: {
    Navbar,
    Hero,
    About,
    Services,
    Team
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
