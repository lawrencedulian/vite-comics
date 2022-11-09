<script>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import ComicsBooks from './components/ComicsBooks.vue';

export default {
  components: {
    AppHeader,
    AppFooter,
    ComicsBooks
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <ComicsBooks />
  </main>
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
</style>