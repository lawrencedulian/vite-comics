<script>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import AppHeaderVue from './components/AppHeader.vue';
import MainContentVue from './components/MainContent.vue';
import AppFooterVue from './components/AppFooter.vue';

export default {
  components: {
    AppHeaderVue,
    AppFooterVue,
    MainContentVue
  }
}
</script>

<template>
  <AppHeaderVue />
  <MainContentVue />
  <AppFooterVue />
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
</style>
