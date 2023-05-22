<script>
import AppHeader from "./components/AppHeader.vue";
import AppProducts from "./components/AppProducts.vue";
import AppFooter from "./components/AppFooter.vue";

export default {
  components: {
    AppHeader: AppHeader,
    AppProducts: AppProducts,
    AppFooter: AppFooter,
  },
};
</script>

<template>
  <AppHeader></AppHeader>
  <AppProducts></AppProducts>
  <AppFooter></AppFooter>
</template>

<style lang="scss">
@use "./assets/style/general.scss" as *;
</style>
