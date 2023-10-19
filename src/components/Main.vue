<script>

import Products from './partials/Products.vue'
import Collections from './partials/Collections.vue'

export default {
  name: 'Main',
  components: {
    Products,
    Collections
  }
  
}
</script>

<template>
  
  <Products />
  <Collections />

</template>

<style lang="scss">
@use '../scss/Main.scss';

</style>