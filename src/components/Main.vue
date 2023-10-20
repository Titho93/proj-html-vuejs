<script>

import Products from './partials/Products.vue';
import Collections from './partials/Collections.vue';
import Bestseller from './partials/Bestseller.vue';
import Offer from './partials/Offer.vue';
import Newarrivals from './partials/Newarrivals.vue';
import Reviews from './partials/Reviews.vue';
import Ourblog from './partials/Ourblog.vue';

export default {
  name: 'Main',
  components: {
    Products,
    Collections,
    Bestseller,
    Offer,
    Newarrivals,
    Reviews,
    Ourblog
  }
  
}
</script>

<template>
  
  <Products />
  <Collections />
  <Bestseller />
  <Offer />
  <Newarrivals />
  <Reviews />
  <Ourblog />

</template>

<style lang="scss">
@use '../scss/Main.scss';

</style>