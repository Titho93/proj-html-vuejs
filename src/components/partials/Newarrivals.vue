<script>

export default {
  name: 'Newarrivals',
  data () {
    return {
      cards: [
      'black_elegant_leather_jacket-400x520.jpg',
      'hipster_black_top-400x520.jpg',
      'black_leather_suit-400x520.jpg',
      'spring_printed_dress-400x520.jpg',
      'modern_love_tee-400x520.jpg'
      ]
    }
  }
  
}
</script>

<template>
  
    <div class="container-main">
        <div class="fp">
            <div class="sectionTitle d-flex">
            <div class="stripe"></div>
            <h2><strong>New Arrivals</strong></h2>
            <div class="stripe"></div>
            </div>
            <p>Brand new product from top designers</p>
        </div>
    </div>

    <div class="swiper d-flex ">
    <div class="arrow left"><i class="fa-solid fa-chevron-left"></i></div>
    <ul class="d-flex">
      <li v-for="(card,index) in cards"
      :key="index">
        <img :src="`../../assets/${card}`" alt="">
      </li>
    </ul>
    <div class="arrow right"><i class="fa-solid fa-chevron-right"></i></div>
  </div>
</template>

<style lang="scss" scoped>

@use '../../scss/partials/Font.scss' as *;
@use '../../scss/partials/Var.scss' as *;
@use '../../scss/partials/Hover.scss' as *;

.fp {
    text-align: center;
    p {
        padding: 20px 0;
    }
}

.swiper {
    ul {
        padding-top: 40px;
        list-style: none;
        li {
            img {
                height: 470px;
            }
        }
    }
}
</style>