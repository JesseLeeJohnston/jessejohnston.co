<template>
  <section>
    <Nav></Nav>
    <div class="section">
    <div class="columns">
      <div class="column">
        <p>Hi, I’m Jesse, a UX Designer with a passion for building web applications that customers love to use. I believe rapid prototyping and feedback cycles help achieve the best end product.</p>
      </div>
      <div class="column">
        <!-- LEAVE EMPTY -->
      </div>
    </div>
    </div>
    <div class="section">
      <PortfolioItem></PortfolioItem>
      <PortfolioItem></PortfolioItem>
      <PortfolioItem></PortfolioItem>
    </div>
    <Footer></Footer>
  </section>
</template>

<script>
import AppLogo from '~/components/AppLogo.vue'
import PortfolioItem from '~/components/PortfolioItem.vue'
import Nav from '~/components/Nav.vue'
import Footer from '~/components/Footer.vue'

export default {
  components: {
    AppLogo,
    PortfolioItem,
    Nav,
    Footer
  }
}
</script>

<style>
  .mb-5 {
    margin-bottom: 5rem;
  }
  .mt-5 {
    margin-top: 5rem;
  }

</style>
