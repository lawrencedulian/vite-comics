<script>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import AppHeader from './components/AppHeader.vue';
import ComicsBooks from './components/ComicsBooks.vue';
import AppShop from './components/AppShop.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  components: {
    AppHeader,
    ComicsBooks,
    AppShop,
    AppFooter
  }
}
</script>

<template>
  <AppHeader />
  <main>
    <ComicsBooks />
    <AppShop />
  </main>
  <AppFooter />
</template>

<style lang="scss">
@use "./styles/general.scss" as *;
</style>