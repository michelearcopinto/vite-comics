<script>
import NavBar from "./components/header/NavBar.vue";
import HeaderFooter from "./components/footer/HeaderFooter.vue";
import MainFooter from "./components/footer/MainFooter.vue";
import FooterFooter from "./components/footer/FooterFooter.vue";

export default {
  components: {
    NavBar,
    HeaderFooter,
    MainFooter,
    FooterFooter,
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
  <FooterFooter />
</template>

<style lang="scss">
@use "./styles/general.scss";
</style>
