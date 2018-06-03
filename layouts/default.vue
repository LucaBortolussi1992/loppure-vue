<template>
  <div id="app">
    <the-navbar/>
    <nuxt/>
    <div class="container is-widescreen">
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
