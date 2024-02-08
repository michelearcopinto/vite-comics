<script>
export default {
  name: "HeaderFooter",
  data() {
    return {
      ctaBoxes: [
        {
          pathImg: "./src/assets/img/buy-comics-digital-comics.png",
          text: "digital comics",
        },
        {
          pathImg: "./src/assets/img/buy-comics-merchandise.png",
          text: "dc merchandise",
        },
        {
          pathImg: "./src/assets/img/buy-comics-subscriptions.png",
          text: "subscription",
        },
        {
          pathImg: "./src/assets/img/buy-comics-shop-locator.png",
          text: "comic shop locator",
        },
        {
          pathImg: "./src/assets/img/buy-dc-power-visa.svg",
          text: "dc power visa",
        },
      ],
    };
  },
  methods: {},
};
</script>

<template>
  <section>
    <div class="container">
      <div v-for="(element, index) in ctaBoxes" key="index">
        <figure>
          <img :src="element.pathImg" :alt="index + 1" />
        </figure>
        <span
          ><a href="">{{ element.text }}</a></span
        >
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;
@use "../../styles/partials/mixins" as *;

section {
  background-color: $color-active-link;
  color: white;
  font-size: 30px;
  font-weight: 700;
  padding-block: 50px;

  .container {
    display: flex;
    align-items: center;
    justify-content: space-evenly;

    div {
      display: flex;
      align-items: center;
      gap: 15px;

      figure {
        display: flex;
        align-items: center;

        img {
          height: 50px;
          max-width: 50px;
        }
      }

      span {
        display: flex;
        align-items: center;

        a {
          text-transform: uppercase;
          font-size: 20px;
          font-weight: 400;
        }
      }
    }
  }
}
</style>
