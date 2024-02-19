<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppSignup from './components/AppSignup.vue';

export default {
  data() {
    return {
    }
  },

  components: { AppHeader, AppSignup, AppMain, AppFooter }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppSignup></AppSignup>
  <AppMain></AppMain>
  <AppFooter></AppFooter>
</template>

<style lang="scss">
@use './styles/generals.scss';
</style>
