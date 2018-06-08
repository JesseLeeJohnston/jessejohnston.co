<template>
<div class="mt-5">
    <div class="columns row-center-vertical">
        <div class="column">
            <h2 class="title">{{project.title}}</h2>
            <p>{{ project.subtitle }}</p>
            <a v-bind:href="project.url" class="button is-primary">View Project</a>
        </div>
        <div class="column">
            <img :src="project.image" alt="">
        </div>
    </div>
</div>
</template>
<script>
export default {
  props: {
    project: {
      type: Object
    }
  }
};
</script>
<style type="scss" scoped>
@media (min-width: 769px) {
  .row-center-vertical {
    display: flex;
    align-items: center;
    justify-content: center;
  }
}
</style>
