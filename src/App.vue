<script>
import NavBar from "./components/header/NavBar.vue";
import HeaderFooter from "./components/footer/HeaderFooter.vue";
import MainFooter from "./components/footer/MainFooter.vue";

export default {
  components: {
    NavBar,
    HeaderFooter,
    MainFooter,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<template>
  <NavBar />
  <HeaderFooter />
  <MainFooter />
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
