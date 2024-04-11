<script>
  import AppHeader from './components/AppHeader.vue';
  import AppHero from './components/AppHero.vue';
  import AppMainNav from './components/AppMainNav.vue';
  import AppFooterTop from './components/AppFooterTop.vue';
  
 export default {
  components: { 
    AppHeader,
    AppHero,
    AppMainNav,
    AppFooterTop,
  
  }
 }

</script>

<template>
    <AppHeader></AppHeader>
    <main>
      <AppHero></AppHero>
      <AppMainNav></AppMainNav>
    </main>
    <AppFooterTop></AppFooterTop>
</template>

<style lang="scss">
  @use './style/generic';
</style>
