<template>
  <aside class="sidebar">
    <!--<rubriche/>-->
    <take-it-out/>
  </aside>

</template>

<script>
  import TakeItOut from '../element/TakeItOut'
  import Rubriche from '../element/rubriche2'

  export default {
    name: 'RightSidebar',
    components: {
      Rubriche,
      TakeItOut,
    },
  }
</script>

<style lang="scss" scoped>

</style>
