<script>

import Products from './partials/Products.vue';
import Collections from './partials/Collections.vue';
import Bestseller from './partials/Bestseller.vue';
import Offer from './partials/Offer.vue';
import Newarrivals from './partials/Newarrivals.vue';
import Reviews from './partials/Reviews.vue';
import Ourblog from './partials/Ourblog.vue';
import Recap from './partials/Recap.vue';

export default {
  name: 'Main',
  components: {
    Products,
    Collections,
    Bestseller,
    Offer,
    Newarrivals,
    Reviews,
    Ourblog,
    Recap
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
  <Recap />

</template>

<style lang="scss">
@use '../scss/Main.scss';

</style>