<template>
  <div class="block-container">
    <img
      class="card"
      v-for="(block, i) in blocks"
      :key="i"
      :src="block"
      alt=""
    />
    <div class="apici">
      <img class="palloncino" src="/svg/svg-7.svg" alt="" />
      <img class="shop" src="/svg/svg-6.svg" alt="" />
    </div>
    <div class="arrow-up1">
      <a href="#">&UpArrow;</a>
    </div>
    <div class="arrow-up2"><a href="#">&UpArrow;</a></div>
  </div>
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
      blocks: [
        `/img/h-2-port-img-1.jpg`,
        `/img/h-2-port-img-2.jpg`,
        `/img/h-2-port-img-3.jpg`,
        `/img/h-2-port-img-4.jpg`,
        `/img/h-2-port-img-5.jpg`,
        `/img/h-2-port-img-6.jpg`,
      ],
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
.block-container {
  display: flex;
  flex-wrap: wrap;
  position: relative;
  .card {
    width: calc(100% / 3);
    cursor: pointer;
  }
  .palloncino,
  .shop {
    width: 48px;
    padding: 9px;
    cursor: pointer;
  }
  .apici {
    position: absolute;
    right: 0;
    top: 134px;
  }
  .palloncino {
    background-color: red;
    margin-bottom: 9px;
  }
  .shop {
    background-color: white;
  }
}
.arrow-up1,
.arrow-up2 {
  background-color: #c0e1cf;
  cursor: pointer;
  width: 45px;
  aspect-ratio: 1/1;
  display: flex;
  align-items: center;
  justify-content: center;
  position: absolute;
  right: 21px;
}
.arrow-up1 {
  bottom: 21px;
}
.arrow-up2 {
  bottom: 445px;
}
</style>
