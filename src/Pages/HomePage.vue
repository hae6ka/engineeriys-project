<template>
  <Header username="Еще не вошел :(" />

  <Main id="main" />

  <Soon id="shop" title="Магазин скоро появится!" />

  <Soon id="news" title="Новости скоро появятся!" />

  <Footer />
</template>

<script>
import Header from "../components/Header.vue";
import Main from "../components/Main.vue";
import Soon from "../components/Soon.vue";
import Footer from "../components/Footer.vue";

export default {
  name: "HomePage",
  components: {
    Header,
    Main,
    Soon,
    Footer
  },
};
</script>

<style lang="scss"></style>
