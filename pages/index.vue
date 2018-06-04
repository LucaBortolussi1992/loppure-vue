<template>
    <div id="home">
      <header-test/>
      <!--<the-hader/>-->
      <div class="container">
        <main class="columns">
          <div class="column is-2-fullhd is-2-widescreen">
            <sidebar-left/>
          </div>
          <div class="column is-8-widescreen article-box">
            <card/>
            <hr class="whitespace whitespace--normal">
            <card/>
            <hr class="whitespace whitespace--normal">
            <card/>
          </div>
          <div class="column is-2-widescreen">
            <sidebar-right/>
          </div>
        </main>
      </div>
  </div>
</template>

<script>
  import HeaderTest from '../components/ui/HeaderTest'
  import TheHader from '../components/ui/TheCategoryGrid.vue';
  import SidebarLeft from '../components/layout/SidebarLeft'
  import SidebarRight from '../components/layout/SidebarRight'
  import Card from '../components/ui/Card'

export default {
  components: {
    Card,
    TheHader,
    SidebarLeft,
    SidebarRight,
    HeaderTest
  }
}
</script>

<style lang="scss" scoped>
  main {
    padding-top: 3rem;
  }
</style>
