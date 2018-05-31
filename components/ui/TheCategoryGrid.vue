<template>
  <header>
    <div class="columns is-multiline">
      <div class="column is-one-fifths has-text-centered">
        <div class="category-grid category-grid--gusti">
          <div class="category-grid__image">
            <img :src="LogoGusti" alt="">
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
          <div class="category-grid__image">
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
          <div class="category-grid__image">
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
          <div class="category-grid__image">
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
          <div class="category-grid__image">
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
  import LogoGusti from '../../assets/logo_category/loppure-gusti-della-terra.svg';
  import LogoPausa from '../../assets/logo_category/loppure-pausa-caffe.svg';
  import LogoRadici from '../../assets/logo_category/loppure-radici-nel-tempo.svg';
  import LogoVoli from '../../assets/logo_category/loppure-voli-sul-territorio.svg';
  import LogoPensieri from '../../assets/logo_category/loppure-pensieri-tra-le-pagine.svg';

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

  .category-grid {
    &--gusti {
      &:hover {
        background-color: $red;
      }
    }
    &--voli {
      &:hover {
        background-color: $green;
      }
    }
    &--radici {
      &:hover {
        background-color: $yellow;
      }
    }
    &--pausa {
      &:hover {
        background-color: $brown;
      }
    }
    &--pensieri {
      &:hover {
        background-color: $purple;
      }
    }

    &__image {
      display: block;
      & img {
        max-width: 60px;
        margin-bottom: 1rem;
      }
    }

    &__title {
      /*padding-bottom: 1rem;*/
      /*border-bottom: 2px solid;*/

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

      &__image {
        display: block;
        & img {
          max-width: 60px;
          margin-bottom: 1rem;
        }
    }

    &__content {
      padding-left: 2rem;
      padding-right: 2rem;
    }

  }
</style>
