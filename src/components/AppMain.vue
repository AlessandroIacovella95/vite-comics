<script>
import AppCards from "./AppCards.vue";
import json from "../../dc-comics.json";

export default {
  components: {
    AppCards,
  },
  data() {
    return {
      cards: json,
    };
  },
};
</script>

<template>
  <div class="cards_container">
    <AppCards v-for="(card, index) in cards" :key="index" :card="card" />
  </div>
</template>

<style lang="scss" scoped>
.cards_container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 0.8rem;
  padding: 20px 0;
  margin: 0 15%;
}
</style>
