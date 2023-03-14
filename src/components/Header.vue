<template>
  <header>
    <div class="logo">
      <img src="/img/logo-sidearea-1.png" alt="" />
    </div>
    <div class="menu">
      <ul class="menu-items">
        <li v-for="(nav, i) in navItems" :key="i">
          <a href="#">{{ nav }}</a>
          <div class="dropdown">
            <ul id="submenu">
              <li v-for="(home, i) in homes" :key="i">
                <a href="#">{{ home }}</a>
              </li>
            </ul>
          </div>
        </li>
      </ul>
      <img class="dots" src="/svg/svg-1.svg" alt="" />
    </div>
  </header>
</template>

<script>
export default {
  components: {
    // **************************
    // FINE COMPONETS
  },
  // **************************
  data() {
    return {
      navItems: [`home`, `pages`, `portfolio`, `blog`, `shop`, `elements`],
      homes: [`1`, `2`, `1`, `2`, `1`, `2`],
      pages: [`3`, `3`, `3`, `3`, `3`, `3`],
      pages: [`4`, `4`, `4`, `4`, `4`, `4`],
      pages: [`5`, `5`, `5`, `5`, `5`, `5`],
      pages: [`6`, `6`, `6`, `6`, `6`, `6`],
      pages: [`7`, `7`, `7`, `7`, `7`, `7`],
      // **************************
      // FINE DATA E RETURN &
    };
  },
  // **************************
  computed: {
    // **************************
    // FINE COMPUTED
  },
  // **************************
  watch: {
    // **************************
    // FINE WATCH
  },
  // **************************
  methods: {
    // **************************
    // FINE METHODS
  },
  // **************************
};
</script>

<style lang="scss" scoped>
@use "../style/partials//variables" as *;
header {
  padding: 15px 40px 20px 40px;
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.logo {
  cursor: pointer;
}
.menu {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 53px;
  .menu-items {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 53px;
    text-transform: uppercase;
    font-weight: bold;
    margin-top: 15px;
  }
}
a {
  color: black !important;
  text-decoration: none;
}
.dropdown ul {
  background-color: bisque;
  list-style: none;
  //   width: 300px;
  padding: 5px;
}

#submenu {
  opacity: 0;
  position: absolute;
  top: 35px;
  z-index: 1;
  visibility: hidden;
}
li:hover ul#submenu {
  opacity: 1;
  top: 25px;
  right: 0;
  visibility: visible;
  //   display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
</style>
