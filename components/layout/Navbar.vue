<template>
  <nav class="navbar has-shadow is-fixed-top">
    <div class="container is-widescreen">
      <div class="navbar-brand">
        <a class="navbar-item" href="https://bulma.io">
          <img src="https://bulma.io/images/bulma-logo.png" alt="Bulma: a modern CSS framework based on Flexbox" width="112" height="28">
        </a>
        <div class="navbar-burger burger" data-target="navbarExampleTransparentExample">
          <span></span>
          <span></span>
          <span></span>
        </div>
      </div>

      <div id="navbarExampleTransparentExample" class="navbar-menu">
      </div>
      <div class="navbar-start">
      </div>

      <div class="navbar-end">
        <a class="navbar-item" href="">
          Home
        </a>
        <a class="navbar-item" href="">
          Chi Siamo
        </a>
        <a class="navbar-item" href="">
          Contatti
        </a>
      </div>
    </div>
  </nav>
</template>

<script>
  export default {
    name: 'Navbar'
  }
</script>

<style lang="scss" scoped>
</style>
