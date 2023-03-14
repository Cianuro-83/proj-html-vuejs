<template>
  <Header />
  <CardBlock />
  <WorkingProcess />
  <WorkWithUs />
  <Example />
  <Footer />
</template>

<script>
import CardBlock from "./components/CardBlock.vue";
import WorkWithUs from "./components/WorkWithUs.vue";
import Header from "./components/Header.vue";
import WorkingProcess from "./components/WorkingProcess.vue";
import Example from "./components/Example.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    CardBlock,
    WorkWithUs,
    Header,
    WorkingProcess,
    Example,
    Footer,
    // **************************
    // FINE COMPONETS
  },
  // **************************
};
</script>

<style lang="scss">
@use "./style/general.scss";
</style>
