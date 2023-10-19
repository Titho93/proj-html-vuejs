<script>

import Headertop from './partials/Headertop.vue'
import Headerbottom from './partials/Headerbottom.vue'

export default {
  name: 'Header',
  components: {
    Headertop,
    Headerbottom
  }
  
}
</script>

<template>

  <div class="container">
    
    <Headertop />
    <Headerbottom />
       
  </div>
</template>

<style lang="scss">


</style>