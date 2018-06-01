<template>
  <div class="mounth-list">
    <h3 class="list-header subtitle">Gli ultimi mesi</h3>
    <ul class="">
      <li class="mounth-list__item active">Giugno</li>
      <li class="mounth-list__item ">Maggio</li>
      <li class="mounth-list__item ">Aprile</li>
    </ul>
  </div>
</template>

<script>
  export default {
    name: 'mounth'
  }
</script>

<style lang="scss" scoped>
  @import "../../style/variables";

  .mounth-list__item {
    padding: 1rem;
    margin-left: 30%;
    border-left: 1px solid $primary;

    &::before {
      content: '\25CF';
      font-size: 2rem;
      color: #40484c;
      position: relative;
      left: -1.6rem;
      bottom: 0.5rem;
      vertical-align: middle;
    }

    &.active {
      &:nth-child(1):before {
        color: $faded-red;
      }
      &:nth-child(2):before {
        color: $faded-green;
      }
      &:nth-child(3):before {
        color: $faded-yellow;
      }
      &:nth-child(3):before {
        color: $faded-brown;
      }
      &:nth-child(3):before {
        color: $faded-purple;
      }
    }
  }
</style>
