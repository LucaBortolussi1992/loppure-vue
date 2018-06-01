<template>
  <div class="city-list">
    <h3 class="list-header subtitle">Città</h3>
    <div class="city-list_city">
      <img :src="pordenone" alt="">
    </div>
    <div class="city-list_city">
      <img :src="gorizia" alt="">
    </div>
    <div class="city-list_city">
      <img :src="treviso" alt="">
    </div>
    <div class="city-list_city">
      <img :src="trieste" alt="">
    </div>
    <div class="city-list_city">
      <img :src="udine" alt="">
    </div>
    <hr class="whitespace whitespace--normal">
    <ul class="">
      <li class="city-list__item" :style="{ backgroundImage: `url(${gorizia})`}">Pordenone</li>
      <li class="city-list__item" :style="{ backgroundImage: `url(${pordenone})`}">Udine</li>
      <li class="city-list__item" :style="{ backgroundImage: `url(${treviso})`}">Gorizia</li>
      <li class="city-list__item" :style="{ backgroundImage: `url(${trieste})`}">Trieste</li>
      <li class="city-list__item" :style="{ backgroundImage: `url(${udine})`}">Treviso</li>
    </ul>
  </div>
</template>

<script>
  import gorizia from  '../../assets/logos_city/citta-gorizia.svg'
  import pordenone from  '../../assets/logos_city/citta-pordenone.svg'
  import treviso from  '../../assets/logos_city/citta-treviso.svg'
  import trieste from  '../../assets/logos_city/citta-trieste.svg'
  import udine from  '../../assets/logos_city/citta-udine.svg'

  export default {
    name: 'CityList',
    data() {
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
  @import "../../style/variables";

  .city-list {
    text-align: center;
  }

  .city-list__item {
    background-size: cover;
    background-position: center center ;
    padding: 1rem 1rem 1rem 0;
    margin-bottom: 1rem;
  }

  .city-list_city {
    margin: 1rem auto;
    position: relative;
    &::after {
      content: 'Pordenone';
      color: white;
      position: absolute;
      top: 50%;
      left: 0;
      right: 0;
    }
    &:before {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      right: 0;
      background-color: #40484c;
      width: 100%;
      height: 100%;
      opacity: 0.3;
    }
  }

  img {
    width: 200px;
  }
</style>
