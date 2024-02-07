<script>
export default {
  name: "MainFooter",
  data() {
    return {
      dcComicsFirst: [
        "characters",
        "comics",
        "movies",
        "tv",
        "games",
        "videos",
        "news",
      ],
      shopSecond: ["shop DC", "shop DC collectibles"],
      dcThird: [
        "terms of use",
        "privacy policy (new)",
        "ad choices",
        "advertising",
        "jobs",
        "subscriptions",
        "talent workshops",
        "CPSC certificates",
        "ratings",
        "shop help",
        "contact us",
      ],
      sitesFourth: [
        "DC",
        "MAD magazine",
        "DC kids",
        "DC universe",
        "DC power visa",
      ],
    };
  },
  methods: {},
};
</script>

<template>
  <section>
    <div class="container">
      <div>
        <div>
          <h2>dc comics</h2>
          <ul>
            <li v-for="element in dcComicsFirst">
              <a href="">{{ element }}</a>
            </li>
          </ul>

          <h2>shop</h2>
          <ul>
            <li v-for="element in shopSecond">
              <a href="">{{ element }}</a>
            </li>
          </ul>
        </div>
        <div>
          <h2>dc</h2>
          <ul>
            <li v-for="element in dcThird">
              <a href="">{{ element }}</a>
            </li>
          </ul>
        </div>
        <div>
          <h2>sites</h2>
          <ul>
            <li v-for="element in sitesFourth">
              <a href="">{{ element }}</a>
            </li>
          </ul>
        </div>
      </div>
      <figure></figure>
    </div>
  </section>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;
@use "../../styles/partials/mixins" as *;

section {
  background-image: url("../../assets/img/footer-bg.jpg");
  background-size: cover;
  background-repeat: no-repeat;
  color: white;

  .container {
    display: flex;
    justify-content: space-between;

    figure {
      background-image: url("../../assets/img/dc-logo-bg.png");
      background-position: 0 60%;
      width: 563px;
      height: 390px;
    }

    div {
      padding-top: 20px;
      display: flex;
      column-gap: 30px;

      div {
        flex-direction: column;

        h2 {
          text-transform: uppercase;
          margin-bottom: 10px;
        }

        ul {
          margin-bottom: 20px;

          li {
            margin-bottom: 4px;

            a {
              color: rgba($color: #ffffff, $alpha: 0.5);
              text-transform: capitalize;
            }
          }
        }
      }
    }
  }
}
</style>
