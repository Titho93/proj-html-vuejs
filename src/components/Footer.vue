<script>

import Send from './partials/Send.vue';
import Repilogue from './partials/Repilogue.vue';

export default {
  name: 'Footer',
  components: {
    Send,
    Repilogue
  }
}

</script>

<template>

<Send />
<Repilogue />
  
</template>

<style lang="scss">
@use '../scss/Main.scss';


</style>