<template>
    <div id="home">
      <div class="container is-widescreen">
        <the-hader/>
        <main class="columns">
          <div class="column is-one-fifth"><sidebar-left/></div>
          <div class="column is-three-fifths article-box">
            <article>Cia</article>
            <article>fdsf</article>
            <article>fdsfds</article>
          </div>
          <!--<div class="column is-one-fifth"><sidebar-right/></div>-->
        </main>
      </div>
  </div>
</template>

<script>
  import TheHader from '../components/ui/TheCategoryGrid.vue';
  import SidebarLeft from '../components/layout/SidebarLeft'
  import SidebarRight from '../components/layout/SidebarRight'

export default {
  components: {
    TheHader,
    SidebarLeft,
    SidebarRight
  }
}
</script>

<style lang="scss" scoped>
  main {
    padding-top: 3rem;
  }
</style>
