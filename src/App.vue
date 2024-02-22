<script>
import { store } from './store';
import AppHeader from './components/AppHeader.vue';
import AppTrainers from './components/AppTrainers.vue';
import AppFooter from './components/AppFooter.vue';
import AppSignup from './components/AppSignup.vue';
import AppIcons from './components/AppIcons.vue';
import AppTestimonials from './components/AppTestimonials.vue';
import AppNews from './components/AppNews.vue';
import AppLinks from './components/AppLinks.vue';
import AppModal from './components/AppModal.vue';

export default {
  data() {
    return {
      store,
    }
  },

  components: { AppHeader, AppSignup, AppIcons, AppTestimonials, AppTrainers, AppNews, AppFooter, AppLinks, AppModal }
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
  <AppModal v-if="store.modal.show"></AppModal>
</template>

<style lang="scss">
@use './styles/generals.scss';
</style>
