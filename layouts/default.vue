<template>
  <div id="app">
    <the-navbar/>
    <div class="container is-widescreen">
      <nuxt/>
    </div>
  </div>
</template>

<script>
  import TheNavbar from '../components/layout/Navbar.vue';
  export default {
    components: {
      TheNavbar
    }
  }
</script>

<style lang="scss">
  body,
  html{
    padding-top: 3.25rem;
  }
</style>
