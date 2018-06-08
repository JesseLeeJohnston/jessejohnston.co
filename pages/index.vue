<template>
  <div>
    <div class="container">
      <div class="columns mt-4">
        <div class="column">
          <p>Hi, I’m Jesse, a UX Designer with a passion for building web applications that customers love to use. I believe rapid prototyping and feedback cycles help achieve the best end product.</p>
        </div>
        <div class="column">
          <!-- LEAVE EMPTY -->
        </div>
      </div>
      <div class="mt-5">
        <PortfolioItem v-for="project in projects" v-bind:project="project" v-bind:key="project.id"></PortfolioItem>
      </div>
    </div>
  </div>
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
        },
        {
          title: "Cully Movie Bot",
          subtitle: "A chatbot channel to help movie theatres sell tickets.",
          url: "/portfolio/cully-chatbot",
          image: "http://placehold.it/600x300"
        },
        {
          title: "ResponseTek Dashboard",
          subtitle: "A reporting platform for voice of customer programs.",
          url: "/portfolio/responsetek-dashboard",
          image: "http://placehold.it/600x300"
        },
        {
          title: "ResponseTek Surveys",
          subtitle: "A survey platform for voice of customer programs.",
          url: "/portfolio/responsetek-surveys",
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
