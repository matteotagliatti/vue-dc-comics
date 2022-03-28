<template>
  <div>
    <main>
      <div class="container">
        <h1>Content goes here</h1>
      </div>
    </main>
    <LinskDiv />
  </div>
</template>

<script>
import LinskDiv from "./Links.vue";

export default {
  name: "MainDiv",
  components: {
    LinskDiv,
  },
};
</script>

<style scoped lang="scss">
main {
  padding: 3rem 0;
  background-color: black;

  h1 {
    color: white;
    font-weight: bold;
  }
}
</style>
