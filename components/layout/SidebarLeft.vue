<template>
  <aside class="sidebar">
    <city/>
    <hr class="whitespace whitespace--normal">
    <mounth/>
  </aside>

</template>

<script>
  // import City from '../element/City'
  import City from '../element/City2'
  import Mounth from '../element/Mounth'

  export default {
    name: 'LeftSidebar',
    components: {
      Mounth,
      City
    },
  }
</script>

<style lang="scss" scoped>

</style>
