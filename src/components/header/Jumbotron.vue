<script>
export default {
  name: "Jumbotron",
  data() {
    return {};
  },
  methods: {},
};
</script>

<template>
  <figure>
    <img src="../../assets/img/jumbotron.jpg" alt="jumbotron" />
  </figure>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;
@use "../../styles/partials/mixins" as *;

figure {
  background-color: black;
  color: white;
  font-size: 30px;
  font-weight: 700;
  height: 400px;
  overflow: hidden;

  img {
  }
}
</style>
