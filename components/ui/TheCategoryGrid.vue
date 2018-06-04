<template>
  <div class="container">
    <div class="columns is-multiline">
      <div class="column is-one-fifth has-text-centered">
        <div class="category-grid category-grid--gusti">
          <div class="category-grid__image category-grid__image--gusti">
            <figure class="image">
              <img :src="LogoGusti" alt="">
            </figure>
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Gusti della Terra</nuxt-link>
          </div>
          <div class="category-grid__content">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Placeat, quae.</p>
          </div>
          <a class="category-grid__link category-grid__link--gusti has-text-centered">Vai alla Rubrica</a>
        </div>
      </div>
      <div class="column is-one-fifth has-text-centered">
        <div class="category-grid category-grid--voli">
          <div class="category-grid__image category-grid__image--voli">
            <figure class="image">
              <img :src="LogoVoli" alt="">
            </figure>
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Voli sul territorio</nuxt-link>
          </div>
          <div class="category-grid__content">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Incidunt, voluptate.
          </div>
        </div>
      </div>
      <div class="column is-one-fifth has-text-centered">
        <div class="category-grid category-grid--radici">
          <div class="category-grid__image category-grid__image--radici">
            <figure class="image">
              <img :src="LogoRadici" alt="">
            </figure>
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Radici nel tempo</nuxt-link>
          </div>
          <div class="category-grid__content">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Molestiae, rerum?
          </div>
        </div>
      </div>
      <div class="column is-one-fifth has-text-centered">
        <div class="category-grid category-grid--pausa">
          <div class="category-grid__image category-grid__image--pausa">
            <figure class="image">
              <img :src="LogoPausa" alt="">
            </figure>
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Pausa caffè</nuxt-link>
          </div>
          <div class="category-grid__content">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nam, voluptatum.
          </div>
        </div>
      </div>
      <div class="column is-one-fifth has-text-centered">
        <div class="category-grid category-grid--pensieri">
          <div class="category-grid__image category-grid__image--pensieri">
            <figure class="image">
              <img :src="LogoPensieri" alt="">
            </figure>
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
  </div>
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
    /*padding: 2rem;*/
  }

  .category-grid {
    border-radius: 3px;
    padding: 2rem;
    overflow: hidden;
    background-color: white;

    &:hover .category-grid__image img {
      transform: scale(1.2);
    }

    &__image {
      display: block;
      max-width: 5rem;
      padding: 1rem;
      margin: 0 auto;

      & img {
        max-width: 60px;
        margin: 0 auto;
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
      padding-top: 3rem;

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
      /*display: none;*/
      background-color: $white;
      padding-bottom: 1rem;
    }

    &__link {
      text-decoration: underline;
      &--gusti {
        color: $red;
      }
      &--voli {
        color: $green;
      }
      &--radici {
        color: $yellow;
      }
      &--pausa {
        color: $brown;
      }
      &--pensieri {
        color: $purple;
      }
    }

  }
</style>
