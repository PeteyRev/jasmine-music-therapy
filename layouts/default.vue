<template>
  <div class="has-navbar-fixed-top">
    <Header />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
import Header from "~/components/Header.vue";
import Footer from "~/components/Footer.vue";

export default {
  name: "Home",
  components: {
    Header,
    Footer
  },
  head: {
    htmlAttrs: {
      class: "has-navbar-fixed-top"
    }
  }
};
</script>
