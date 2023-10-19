<script>

import Products from './partials/Products.vue';
import Collections from './partials/Collections.vue';
import Bestseller from './partials/Bestseller.vue';

export default {
  name: 'Main',
  components: {
    Products,
    Collections,
    Bestseller
  }
  
}
</script>

<template>
  
  <Products />
  <Collections />
  <Bestseller />

</template>

<style lang="scss">
@use '../scss/Main.scss';

</style>