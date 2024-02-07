<script>
// import

export default {
  name: "NavBar",
};
</script>

<template>
  <h1>Hi I'm component</h1>
</template>

<style lang="scss" scoped>
@use "@/src/styles/partials/variables" as *;
@use "@/src/styles/partials/mixins" as *;

h1 {
  color: $font-color-second;
  @include main-font-start;
}
</style>
