<template>
  <footer>
    <div class="footer-up">
      <div class="container"></div>
    </div>
    <div class="footer-down">
      <div class="container">
        <a href="#">SIGN-UP DOWN</a>
        <div id="social">
          <span>Follow Us</span>
          <img
            v-for="(social, index) in socialImg"
            :src="social.img"
            :alt="social.text"
            :key="index"
          />
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterDiv",
  data() {
    return {
      socialImg: [
        {
          text: "Facebook",
          img: require("../assets/img/footer-facebook.png"),
          url: "#",
        },
        {
          text: "Twitter",
          img: require("../assets/img/footer-twitter.png"),
          url: "#",
        },
        {
          text: "Youtube",
          img: require("../assets/img/footer-youtube.png"),
          url: "#",
        },
        {
          text: "Pinterest",
          img: require("../assets/img/footer-pinterest.png"),
          url: "#",
        },
        {
          text: "Periscope",
          img: require("../assets/img/footer-periscope.png"),
          url: "#",
        },
      ],
    };
  },
};
</script>

<style scoped lang="scss">
@import "../assets/scss/style.scss";

.footer-up {
  height: 500px;
  background-image: url(../assets/img/footer-bg.jpg);
}

.footer-down {
  padding: 2.2rem 0;
  background-color: #303030;

  .container {
    display: flex;
    justify-content: space-between;
  }

  a {
    padding: 1rem;
    border: 2px solid $blue;
    color: white;
    text-transform: uppercase;
    text-decoration: none;
    font-weight: bold;
  }

  #social {
    display: flex;
    align-items: center;
    gap: 1rem;

    span {
      font-size: 1.3rem;
      font-weight: bold;
      text-transform: uppercase;
      color: $blue;
    }
  }
}
</style>
