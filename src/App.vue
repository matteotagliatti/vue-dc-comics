<template>
  <div id="app">
    <HeaderDiv />
    <MainDiv />
    <FooterDiv />
  </div>
</template>

<script>
import HeaderDiv from "./components/Header.vue";
import MainDiv from "./components/Main.vue";
import FooterDiv from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    HeaderDiv,
    MainDiv,
    FooterDiv,
  },
};
</script>

<style lang="scss">
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

#app {
  max-width: 1100px;
  margin: 0 auto;
  font-family: sans-serif;
}

li {
  list-style: none;
}
</style>
