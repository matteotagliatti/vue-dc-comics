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
@import "./assets/scss/style.scss";
</style>
