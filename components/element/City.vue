<template>
  <div class="city-list">
    <h3 class="list-header subtitle">Città</h3>
    <ul class="">
      <li class="city-list__item">Pordenone</li>
      <li class="city-list__item ">Udine</li>
      <li class="city-list__item ">Gorizia</li>
      <li class="city-list__item ">Trieste</li>
      <li class="city-list__item ">Treviso</li>
    </ul>
  </div>
</template>

<script>
  export default {
    name: ''
  }
</script>

<style lang="scss" scoped>
  @import "../../style/variables";

  .city-list__item {
    padding: 1rem 1rem 1rem 0;
    margin-left: 30%;
  }
</style>
