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

  <div class="container-bt">
    
    <Headertop />
    <Headerbottom />
       
  </div>
</template>

<style lang="scss">

.container-bt {
  width: 70%;
  margin: 0 auto;
}


</style>