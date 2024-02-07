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
    <div class="container">--&gt; Content goes here &lt;--</div>
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
  padding-block: 40px;
}
</style>
