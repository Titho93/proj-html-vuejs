<script>

import Products from './partials/Products.vue'

export default {
  name: 'Main',
  components: {
    Products
  }
  
}
</script>

<template>
  
  <Products />

</template>

<style lang="scss">
@use '../scss/Main.scss';

</style>