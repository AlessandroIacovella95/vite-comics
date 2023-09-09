<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppHeader.vue";
import AppFooter from "./components/AppHeader.vue";

export default {
  components: { AppHeader, AppMain, AppFooter },
};
</script>

<template>
  <div class="wrapper">
    <header>
      <AppHeader />
    </header>
  </div>
</template>

<style lang="scss">
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

.wrapper {
  margin: 0 15%;
}
</style>
