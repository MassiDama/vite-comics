<script>
import AppHeader from './components/AppHeader.vue'
import AppJumbotron from './components/AppJumbotron.vue'
import ListProduct from './components/ListProduct.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  components: {
    AppHeader,
    AppJumbotron,
    ListProduct,
    AppFooter,
  }
}
</script>

<template>
  
  <AppHeader />
  <AppJumbotron />
  <ListProduct />
  <AppFooter />

</template>

<style lang="scss">
</style>
