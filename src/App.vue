<script>
  import AppHeader from './components/AppHeader.vue';
  import AppHero from './components/AppHero.vue';
  import AppMainNav from './components/AppMainNav.vue';
  import AppFooterTop from './components/AppFooterTop.vue';
  import AppFooterBottom from './components/AppFooterBottom.vue';
  
 export default {
  components: { 
    AppHeader,
    AppHero,
    AppMainNav,
    AppFooterTop,
    AppFooterBottom,
  
  }
 }

</script>

<template>
    <AppHeader></AppHeader>
    <main>
      <AppHero></AppHero>
      <AppMainNav></AppMainNav>
    </main>
    <footer>
      <AppFooterTop></AppFooterTop>
      <AppFooterBottom></AppFooterBottom>
    </footer>
</template>

<style lang="scss">
  @use './style/generic';
</style>
