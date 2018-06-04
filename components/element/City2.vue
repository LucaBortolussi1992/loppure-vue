<template>
  <section>
    <h3 class="list-header subtitle">Città</h3>
    <div class="columns is-multiline">
      <div class="column is-half is-half-widescreen has-text-centered">
        <div class="category-grid category-grid--gusti">
          <div class="category-grid__image category-grid__image--gusti">
            <img :src="pordenone" alt="">
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Pordenone</nuxt-link>
          </div>
        </div>
      </div>
      <div class="column is-half is-half-widescreen has-text-centered">
        <div class="category-grid category-grid--voli">
          <div class="category-grid__image category-grid__image--voli">
            <img :src="udine" alt="">
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Udine</nuxt-link>
          </div>
        </div>
      </div>
      <div class="column is-half is-half-widescreen has-text-centered">
        <div class="category-grid category-grid--radici">
          <div class="category-grid__image category-grid__image--radici">
            <img :src="trieste" alt="">
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Trieste</nuxt-link>
          </div>
        </div>
      </div>
      <div class="column is-half is-half-widescreen has-text-centered">
        <div class="category-grid category-grid--pausa">
          <div class="category-grid__image category-grid__image--pausa">
            <img :src="gorizia" alt="">
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Gorizia</nuxt-link>
          </div>
        </div>
      </div>
      <div class="column is-half is-half-widescreen has-text-centered">
        <div class="category-grid category-grid--pensieri">
          <div class="category-grid__image category-grid__image--pensieri">
            <img :src="treviso" alt="">
          </div>
          <div class="category-grid__title title is-5">
            <nuxt-link to="/">Treviso</nuxt-link>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
  import gorizia from '../../assets/logos_city/citta-gorizia.svg'
  import pordenone from '../../assets/logos_city/citta-pordenone.svg'
  import treviso from '../../assets/logos_city/citta-treviso.svg'
  import trieste from '../../assets/logos_city/citta-trieste.svg'
  import udine from '../../assets/logos_city/citta-udine.svg'

  export default {
    data () {
      return {
        gorizia,
        pordenone,
        treviso,
        trieste,
        udine
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "../../style/main";

  .column {
  }

  .category-grid {
    border-radius: 8px;
    overflow: hidden;
    background-color: transparent;

    &:hover .category-grid__image img {
      transform: scale(2);
    }

    &__image {
      min-height: 75px;
      overflow: hidden;
      display: block;

      & img {
        padding-top: 0.8rem;
        margin: 1rem;
        transition: transform 3s ease-in-out;
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
      padding-bottom: 1rem;

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
      background-color: transparent;
      padding-bottom: 1rem;
    }

  }
</style>
