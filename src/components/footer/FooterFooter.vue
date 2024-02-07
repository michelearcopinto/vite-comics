<script>
export default {
  name: "FooterFooter",
  data() {
    return {
      socialImg: [
        "./src/assets/img/footer-facebook.png",
        "./src/assets/img/footer-periscope.png",
        "./src/assets/img/footer-pinterest.png",
        "./src/assets/img/footer-twitter.png",
        "./src/assets/img/footer-youtube.png",
      ],
    };
  },
  methods: {},
};
</script>

<template>
  <section>
    <div class="container">
      <button>sign-up now!</button>
      <div>
        <h3>follow us</h3>
        <div>
          <figure v-for="(element, index) in socialImg">
            <img :src="element" :alt="index + 1" />
          </figure>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;
@use "../../styles/partials/mixins" as *;

section {
  background-color: $color-bg-footer;
  padding-block: 25px;

  div {
    display: flex;
    align-items: center;
    justify-content: space-between;

    button {
      text-transform: uppercase;
      color: white;
      background-color: $color-bg-footer;
      border: 2px solid $color-active-link;
      padding: 10px;
      font-weight: 700;

      &:hover {
        cursor: pointer;
      }
    }

    div {
      display: flex;
      gap: 20px;

      h3 {
        color: $color-active-link;
        text-transform: uppercase;
      }

      div {
        display: flex;

        figure {
          cursor: pointer;
        }
      }
    }
  }
}
</style>
