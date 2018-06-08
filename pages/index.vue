<template>
  <section>
    <div class="container">
    <div class="columns">
      <div class="column">
        <p>Hi, I’m Jesse, a UX Designer with a passion for building web applications that customers love to use. I believe rapid prototyping and feedback cycles help achieve the best end product.</p>
      </div>
      <div class="column">
        <!-- LEAVE EMPTY -->
      </div>
    </div>
    </div>
    <div class="container">
      <PortfolioItem v-for="project in projects" v-bind:project="project" v-bind:key="project.id"></PortfolioItem>
    </div>
    <div class="container">
    </div>
  </section>
</template>

<script>
import PortfolioItem from "~/components/PortfolioItem.vue";

export default {
  data: function() {
    return {
      projects: [
        {
          title: "Buddi",
          subtitle: "A system to help budtenders.",
          url: "/portfolio/buddi",
          image: "http://placehold.it/600x300"
        }
      ]
    };
  },
  components: {
    PortfolioItem
  }
};
</script>

<style>
.mb-5 {
  margin-bottom: 5rem;
}
.mt-5 {
  margin-top: 5rem;
}
</style>
