<template>
    <div id="home">
      <div class="container is-widescreen">
        <the-hader/>
      </div>
  </div>
</template>

<script>
  import TheHader from '../components/ui/TheCategoryGrid.vue';

export default {
  components: {
    TheHader
  }
}
</script>

<style>
  .is-red{
    background-color: red;
  }
</style>
