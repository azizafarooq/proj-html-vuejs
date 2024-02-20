<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import AppSignup from './components/AppSignup.vue';
import AppIcons from './components/AppIcons.vue';
import AppCards from './components/AppCards.vue';

export default {
  data() {
    return {
    }
  },

  components: { AppHeader, AppSignup, AppIcons, AppCards, AppMain, AppFooter }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppSignup></AppSignup>
  <AppIcons></AppIcons>
  <AppCards></AppCards>
  <AppMain></AppMain>
  <AppFooter></AppFooter>
</template>

<style lang="scss">
@use './styles/generals.scss';
</style>
