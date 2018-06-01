<template>
    <div id="home">
      <div class="container is-widescreen">
        <the-hader/>
        <main class="columns">
          <div class="column is-3-fullhd is-3-widescreen"><sidebar-left/></div>
          <div class="column
          is-offset-1-widescreen
          is-4-widescreen
          article-box">
            <card/>
            <hr class="whitespace whitespace--normal">
            <card/>
            <card/>
          </div>
          <div class="column
          is-offset-1-widescreen
          is-3-widescreen"><sidebar-right/></div>
        </main>
      </div>
  </div>
</template>

<script>
  import TheHader from '../components/ui/TheCategoryGrid.vue';
  import SidebarLeft from '../components/layout/SidebarLeft'
  import SidebarRight from '../components/layout/SidebarRight'
  import Card from '../components/ui/Card'

export default {
  components: {
    Card,
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
