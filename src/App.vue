<script>
  import AppHeader from './components/AppHeader.vue';
  import AppHero from './components/AppHero.vue';
  import AppIcons from './components/AppIcons.vue';
  import AppInfo from './components/AppInfo.vue';
  import AppFooter from './components/AppFooter.vue';

  export default {
    components: {
      AppHeader,
      AppHero,
      AppIcons,
      AppInfo,
      AppFooter
    }
  }
</script>

<template>
  <header>
    <AppHeader></AppHeader>
  </header>

  <main>
    <AppHero></AppHero>
    <AppIcons></AppIcons>
    <AppInfo></AppInfo>
  </main>
  
  <footer>
    <AppFooter></AppFooter>
  </footer>
</template>

<style>

</style>