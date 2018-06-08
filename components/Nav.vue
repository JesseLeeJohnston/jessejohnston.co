<template>
<!-- Main container -->
<div class="container">
<nav class="level is-fixed navbar">
  <!-- Left side -->
  <div class="level-left">
    <div class="level-item">
        <div class="navbar-brand">
          <nuxt-link to="/">
            <img src="https://www.jessejohnston.co/images/jjlogo.svg" alt="Jesse Johnston Logo">
          </nuxt-link>
        </div>
    </div>
  </div>
  <!-- Right side -->
  <div class="level-right">
    <p class="level-item"><nuxt-link to="/">Home</nuxt-link></p>
    <p class="level-item"><nuxt-link to="/about">About</nuxt-link></p>
  </div>
</nav>
</div>
</template>

<style>
nav {
  margin: 24px 0;
}
</style>
