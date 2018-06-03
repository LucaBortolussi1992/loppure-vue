<template>
  <header>
    <div class="columns is-multiline">
      <div class="column is-one-fifths has-text-centered">
        <div class="category-grid category-grid--gusti">

          <div class="category-grid__image category-grid__image--gusti">
            <figure class="image is-1by1">
              <img :src="LogoGusti" alt="">
            </figure>
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Gusti della Terra</nuxt-link>
          </div>
          <div class="category-grid__content">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Placeat, quae.</p>
          </div>
        </div>
      </div>
      <div class="column is-one-fifths has-text-centered">
        <div class="category-grid category-grid--voli">
          <div class="category-grid__image category-grid__image--voli">a
            <img :src="LogoVoli" alt="">
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Voli sul territorio</nuxt-link>
          </div>
          <div class="category-grid__content">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Incidunt, voluptate.
          </div>
        </div>
      </div>
      <div class="column is-one-fifths has-text-centered">
        <div class="category-grid category-grid--radici">
          <div class="category-grid__image category-grid__image--radici">
            <img :src="LogoRadici" alt="">
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Radici nel tempo</nuxt-link>
          </div>
          <div class="category-grid__content">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestiae, rerum?
          </div>
        </div>
      </div>
      <div class="column is-one-fifths has-text-centered">
        <div class="category-grid category-grid--pausa">
          <div class="category-grid__image category-grid__image--pausa">
            <img :src="LogoPausa" alt="">
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Pausa caffè</nuxt-link>
          </div>
          <div class="category-grid__content">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nam, voluptatum.
          </div>
        </div>
      </div>
      <div class="column is-one-fifths has-text-centered">
        <div class="category-grid category-grid--pensieri">
          <div class="category-grid__image category-grid__image--pensieri">
            <img :src="LogoPensieri" alt="">
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Pensieri tra le pagine</nuxt-link>
          </div>
          <div class="category-grid__content">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Officia, qui.
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
  import LogoGusti from '../../assets/logos_category/loppure-gusti-della-terra.svg';
  import LogoPausa from '../../assets/logos_category/loppure-pausa-caffe.svg';
  import LogoRadici from '../../assets/logos_category/loppure-radici-nel-tempo.svg';
  import LogoVoli from '../../assets/logos_category/loppure-voli-sul-territorio.svg';
  import LogoPensieri from '../../assets/logos_category/loppure-pensieri-tra-le-pagine.svg';

  export default {
    data() {
      return {
        LogoGusti,
        LogoPausa,
        LogoRadici,
        LogoVoli,
        LogoPensieri
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "../../style/main";

  .column {
    padding: 2rem;
  }

  .category-grid {
    border-radius: 8px;
    overflow: hidden;
    background-color: white;

    &:hover .category-grid__image img {
      transform: scale(1.2);
    }

    &__image {
      display: block;

      & img {
        max-width: 60px;
        margin: 1rem 0;
        transition: transform .3s ease-in-out;
      }

      &--gusti {
        background-color: $faded-red;
      }
      &--voli {
        background-color: $faded-green;
      }
      &--radici {
        background-color: $faded-yellow;
      }
      &--pausa {
        background-color: $faded-brown;
      }
      &--pensieri {
        background-color: $faded-purple;
      }
    }

    &__title {
      padding-top: 1rem;

      & a {
        color: $primary;
      }
      &--gusti {
        border-color: $red;
      }
      &--voli {
        border-color: $green;
      }
      &--radici {
        border-color: $yellow;
      }
      &--pausa {
        border-color: $brown;
      }
      &--pensieri {
        border-color: $purple;
      }
    }

    &__content {
      display: none;
      background-color: $white;
      padding-bottom: 1rem;
    }

  }
</style>
