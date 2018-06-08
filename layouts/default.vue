<template>
  <section class="section">
    <Nav></Nav>
    <div class="container">
      <nuxt/>
    </div>
    <Footer></Footer>
  </section>
</template>
<script>
import Nav from "~/components/Nav.vue";
import Footer from "~/components/Footer.vue";

export default {
  components: {
    Nav,
    Footer
  }
};
</script>
<style lang="scss">
@import "../assets/styles.scss";
.container {
  max-width: 940px;
}
</style>
