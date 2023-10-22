<script>

export default {
  name: 'Brand',
  data () {
    return {
        images: [
            'b_logotype_6.png',
            'b_logotype_7.png',
            'b_logotype_1.png',
            'b_logotype_2.png',
            'b_logotype_3.png'
        ]
    }
  }
}
</script>

<template>
  
  <div class="container-lo">
      <span>BRAND LOGOS</span>
      <div class="logos">
        <ul>
            <li v-for="(image,index) in images"
            :key="index">
                <img :src="`../../assets/${ image }`" alt="">
            </li>
        </ul>
    </div>

  </div>
 

</template>

<style lang="scss" scoped>

@use '../../scss/partials/Font.scss' as *;
@use '../../scss/partials/Var.scss' as *;
@use '../../scss/partials/Hover.scss' as *;

.container-lo {
    width: 100%;
    height: 300px;
    padding-top: 60px;
    text-align: center;
    background-color: $darkwhite-color;
    span {
        letter-spacing: 0.2em;
        padding-left: 30px;
    }
    .logos {
        padding-top: 40px;
        margin: 0 auto;
        width: 70%;
        ul {
            display: flex;
            list-style: none;
            li {
                width: 100%;
            }
        }
    }
}


</style>