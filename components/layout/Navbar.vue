<template>
  <nav class="navbar has-shadow is-fixed-top">
    <div class="container is-widescreen">
      <div class="navbar-brand">
        <nuxt-link class="navbar-item" to="">
          <img :src="logo" alt="loppure" width="112" height="28">
        </nuxt-link>
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
  import logo from '../../assets/loppure_logos/loppure-logo-nero.svg'

  export default {
    name: 'Navbar',
    data() {
      return {
        logo
      }
    }
  }
</script>

<style lang="scss" scoped>
</style>
