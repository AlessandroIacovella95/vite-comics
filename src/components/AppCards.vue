<script>
export default {
  props: {
    card: Object,
  },
};
</script>

<template>
  <div class="card">
    <img :src="card.thumb" :alt="card.series" />
    <h4>{{ card.series }}</h4>
  </div>
</template>

<style lang="scss" scoped>
.card {
  width: 150px;
  color: white;
  font-size: 0.8rem;
  img {
    height: 150px;
    aspect-ratio: 1;
    max-width: 100%;
  }
}
</style>
