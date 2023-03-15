<template>
  <div class="block-container">
    <div class="cianuro" v-for="(block, i) in blocks" :key="i">
      <div class="prova">
        <img class="illustration" :src="block.src" alt="" />
        <p>{{ block.text }}</p>
      </div>
    </div>
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
        {
          src: `/img/h-2-port-img-1.jpg`,
          text: `prova`,
        },
        {
          src: `/img/h-2-port-img-2.jpg`,
          text: `prova`,
        },
        {
          src: `/img/h-2-port-img-3.jpg`,
          text: `prova`,
        },
        {
          src: `/img/h-2-port-img-4.jpg`,
          text: `prova`,
        },
        {
          src: `/img/h-2-port-img-5.jpg`,
          text: `prova`,
        },
        {
          src: `/img/h-2-port-img-6.jpg`,
          text: `prova`,
        },
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
}
.cianuro {
  flex-basis: calc(100% / 3);
}
.prova {
}
</style>
