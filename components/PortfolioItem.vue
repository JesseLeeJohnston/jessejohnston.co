<template>
<div>
    <div class="columns">
        <div class="column">
            <h1 class="title">{{project.title}}</h1>
            <h2 class="subtitle">{{ project.subtitle }}</h2>
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
<style>
</style>
