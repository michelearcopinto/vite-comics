<script>
import ListComics from "../main/ListComics.vue";

export default {
  name: "Jumbotron",
  components: {
    ListComics,
  },
};
</script>

<template>
  <section>
    <figure>
      <img src="../../assets/img/jumbotron.jpg" alt="jumbotron" />
    </figure>
  </section>
  <ListComics />
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;
@use "../../styles/partials/mixins" as *;

figure {
  background-color: black;
  color: white;
  font-size: 30px;
  font-weight: 700;
  height: 350px;
  overflow: hidden;
}
</style>
