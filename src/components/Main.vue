<template>
  <div>
    <main>
      <div class="container">
        <div class="cards">
          <ComicCard
            v-for="(comic, index) in comics"
            :key="index"
            :comicProps="comic"
          />
        </div>
        <div class="load-more">
          <a href="#">Load More</a>
        </div>
      </div>
    </main>
    <LinskDiv />
  </div>
</template>

<script>
import LinskDiv from "./Links.vue";
import ComicCard from "./ComicCard.vue";
import comicsData from "../assets/data/dc-comics.json";

export default {
  name: "MainDiv",
  components: {
    LinskDiv,
    ComicCard,
  },
  data() {
    return {
      comics: comicsData,
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/style.scss";

main {
  padding: 3rem 0;
  background-color: black;

  .cards {
    @include flex-between;
    flex-wrap: wrap;
  }

  .load-more {
    text-align: center;

    a {
      padding: 1rem 3rem;
      text-decoration: none;
      text-transform: uppercase;
      font-weight: bold;
      color: white;
      background-color: $blue;
    }
  }
}
</style>
