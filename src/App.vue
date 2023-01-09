<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppMainBanner from './components/AppMainBanner.vue';

export default {
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppMainBanner,
  }
}

</script>

<template>
  <AppHeader/>

  <AppMain/>
  
  <AppMainBanner/>

  <AppFooter/>

</template>

<style lang="scss">
@use './styles/general.scss' as *;
@use './styles/partials/_variables.scss' as *;
</style>
