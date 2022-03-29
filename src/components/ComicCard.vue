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

  color: white;
  display: flex;
  flex-direction: column;
  gap: 0.8rem;

  img {
    height: 10rem;
    object-fit: cover;
    object-position: top;
  }
}
</style>
