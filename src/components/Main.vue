<script>

import Products from './partials/Products.vue';
import Collections from './partials/Collections.vue';
import Bestseller from './partials/Bestseller.vue';
import Offer from './partials/Offer.vue';

export default {
  name: 'Main',
  components: {
    Products,
    Collections,
    Bestseller,
    Offer
  }
  
}
</script>

<template>
  
  <Products />
  <Collections />
  <Bestseller />
  <Offer />

</template>

<style lang="scss">
@use '../scss/Main.scss';

</style>