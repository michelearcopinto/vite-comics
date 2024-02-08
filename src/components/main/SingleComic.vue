<script>
export default {
  name: "SingleComic",
  props: {
    propPath: String,
    propTitle: String,
  },
  data() {
    return {};
  },
  methods: {},
};
</script>

<template>
  <div>
    <figure>
      <img :src="propPath" :alt="propTitle" />
    </figure>
    <span>{{ propTitle }}</span>
  </div>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;
@use "../../styles/partials/mixins" as *;

div:not(div:first-child) {
  width: calc((100% / 6) - 20px);

  figure {
    aspect-ratio: 1;
    background-size: cover;
    margin-bottom: 15px;
    overflow: hidden;

    &:hover {
      cursor: pointer;
      filter: brightness(50%);
    }
  }
}
</style>
