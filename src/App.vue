<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import { _items } from './data';

export default {
  name: "DC",
  components: {
    AppHeader, AppMain, AppFooter
  },
  data: () => ({
    _items
  }),
};

</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
</template>
  

<style lang="scss" scoped>
@use './assets/scss/style.scss';
</style>
