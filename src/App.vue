<script>
  import AppHeader from './components/AppHeader.vue';
  import AppHero from './components/AppHero.vue';
  import AppMainNav from './components/AppMainNav.vue';
  
 export default {
  components: { 
    AppHeader,
    AppHero,
    AppMainNav,
  
  }
 }

</script>

<template>
    <AppHeader></AppHeader>
    <main>
      <AppHero></AppHero>
      <AppMainNav></AppMainNav>
    </main>
</template>

<style lang="scss">
  @use './style/generic';
</style>
