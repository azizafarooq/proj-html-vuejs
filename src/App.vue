<script>
import AppHeader from './components/AppHeader.vue';
import AppTrainers from './components/AppTrainers.vue';
import AppFooter from './components/AppFooter.vue';
import AppSignup from './components/AppSignup.vue';
import AppIcons from './components/AppIcons.vue';
import AppTestimonials from './components/AppTestimonials.vue';
import AppNews from './components/AppNews.vue';
import AppLinks from './components/AppLinks.vue';

export default {
  data() {
    return {
    }
  },

  components: { AppHeader, AppSignup, AppIcons, AppTestimonials, AppTrainers, AppNews, AppFooter, AppLinks }
}
</script>

<template>
  <AppHeader></AppHeader>
  <AppSignup></AppSignup>
  <AppIcons></AppIcons>
  <AppTestimonials></AppTestimonials>
  <AppTrainers></AppTrainers>
  <AppNews></AppNews>
  <AppFooter> </AppFooter>
  <AppLinks></AppLinks>
</template>

<style lang="scss">
@use './styles/generals.scss';
</style>
