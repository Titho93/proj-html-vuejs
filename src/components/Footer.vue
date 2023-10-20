<script>

import Send from './partials/Send.vue';
import Repilogue from './partials/Repilogue.vue';
import Payment from './partials/Payment.vue';

export default {
  name: 'Footer',
  components: {
    Send,
    Repilogue,
    Payment
  }
}

</script>

<template>

<Send />
<Repilogue />
<Payment />
  
</template>

<style lang="scss">
@use '../scss/Main.scss';


</style>