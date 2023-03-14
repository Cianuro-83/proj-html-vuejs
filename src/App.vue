<template>
  <Header />
  <CardBlock />
  <WorkingProcess />
  <WorkWithUs />
  <Example />
</template>

<script>
import CardBlock from "./components/CardBlock.vue";
import WorkWithUs from "./components/WorkWithUs.vue";
import Header from "./components/Header.vue";
import WorkingProcess from "./components/WorkingProcess.vue";
import Example from "./components/Example.vue";
export default {
  components: {
    CardBlock,
    WorkWithUs,
    Header,
    WorkingProcess,
    Example,
    // **************************
    // FINE COMPONETS
  },
  // **************************
};
</script>

<style lang="scss">
@use "./style/general.scss";
</style>
