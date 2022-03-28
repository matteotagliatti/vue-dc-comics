<template>
  <div>
    <main>
      <div class="container">
        <h1>Content goes here</h1>
      </div>
    </main>
    <div id="links">
      <div class="container">
        <div v-for="(element, index) in links" :key="index">
          <img :src="element.img" :alt="element.text" />
          <span>{{ element.text }}</span>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MainDiv",
  data() {
    return {
      links: [
        {
          text: "Digital comics",
          img: "../assets/img//img/buy-comics-digital-comics.png",
        },
        {
          text: "DC Merchandise",
          img: "../assets/img/buy-comics-merch.png",
        },
        {
          text: "Sybscription",
          img: "../assets/img/buy-comics-subscription.png",
        },
        {
          text: "Comic Shop Locator",
          img: "../assets/img/buy-comics-shop-locator.png",
        },
        {
          text: "DC Power Visa",
          img: "../assets/img/buy-comics-power-visa.png",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/style.scss";

main {
  padding: 3rem 0;
  background-color: black;

  h1 {
    color: white;
    font-weight: bold;
  }
}

#links {
  padding: 3rem 0;
  background-color: $blue;

  .container {
    display: flex;
    align-items: center;

    span {
      color: white;
      text-transform: uppercase;
    }
  }
}
</style>
