<template>
  <section class="takeItOut has-text-centered">
    <h3 class="list-header">Porta l'oppure nella tua città</h3>
    <figure class="takeItOut__img image"><img :src="PortaLoppure" alt=""></figure>
    <button>Scopri come</button>
  </section>
</template>

<script>
  import PortaLoppure from '../../assets/porta-loppure.svg'

  export default {
    name: 'PortaLOppure',
    data () {
      return {
        PortaLoppure
      }
    }
  }
</script>

<style lang="scss" scoped>
  .takeItOut {
    &__img {
      max-width: 150px;
      max-height: 150px;
      margin: 0 auto;
    }
  }
</style>
