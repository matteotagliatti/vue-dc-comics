<template>
  <div>
    <img :src="comicProps.thumb" alt="comicProps.series" />
    <span>{{ comicProps.series }}</span>
  </div>
</template>

<script>
export default {
  name: "ComicCard",
  props: {
    comicProps: Object,
  },
};
</script>

<style lang="scss" scoped>
div {
  margin-bottom: 3rem;
  width: 10rem;
  display: flex;
  flex-direction: column;
  gap: 1rem;
  color: white;

  img {
    height: 10rem;
    object-fit: cover;
    object-position: top;
  }

  span {
    text-transform: uppercase;
  }
}
</style>
