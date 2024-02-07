<script>
import NavBar from "./components/header/NavBar.vue";

export default {
  components: {
    NavBar,
  },
};
</script>

<template>
  <h1>Hello World</h1>

  <NavBar />
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
