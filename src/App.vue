<template>
  <CardBlock />
  <WorkWithUs />
</template>

<script>
import CardBlock from "./components/CardBlock.vue";
import WorkWithUs from "./components/WorkWithUs.vue";
export default {
  components: {
    CardBlock,
    WorkWithUs,
    // **************************
    // FINE COMPONETS
  },
  // **************************
};
</script>

<style lang="scss">
@use "./style/general.scss";
</style>
