<script>
// import

export default {
  name: "NavBar",
  data() {
    return {
      listItems: [
        {
          text: "characters",
          status: false,
        },
        {
          text: "comics",
          status: true,
        },
        {
          text: "movies",
          status: false,
        },
        {
          text: "tv",
          status: false,
        },
        {
          text: "games",
          status: false,
        },
        {
          text: "collectibles",
          status: false,
        },
        {
          text: "videos",
          status: false,
        },
        {
          text: "fans",
          status: false,
        },
        {
          text: "news",
          status: false,
        },
        {
          text: "shop",
          status: false,
        },
      ],
    };
  },
  methods: {},
};
</script>

<template>
  <header>
    <nav>
      <figure>
        <img src="../../assets/img/dc-logo.png" alt="logo-header" />
      </figure>
      <ul>
        <li
          v-for="(element, index) in listItems"
          key="index"
          :class="element.status ? 'active' : ''"
        >
          {{ element.text }}
        </li>
      </ul>
    </nav>
  </header>
</template>

<style lang="scss" scoped>
@use "../../styles/partials/variables" as *;
@use "../../styles/partials/mixins" as *;

header {
  padding-top: 25px;

  nav {
    figure:hover {
      cursor: pointer;
    }

    display: flex;
    align-items: center;
    justify-content: space-evenly;

    ul {
      display: flex;
      text-transform: uppercase;
      font-weight: 700;

      li {
        line-height: 80px;
        padding-inline: 10px;

        &:hover {
          cursor: pointer;
          @include active-link;
        }
      }
    }
  }
}

.active {
  @include active-link;
}
</style>
