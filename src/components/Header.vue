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

  <div class="container-tb">
   
    <Headertop />
    
  </div>

  <Headerbottom />

</template>

<style lang="scss" scoped>

@use '../scss/Main.scss';
@use '../scss/partials/Var.scss' as *;

 .container-tb {
  width: 100%;
  border-bottom: 1px solid $darkwhite-color;
}


</style>