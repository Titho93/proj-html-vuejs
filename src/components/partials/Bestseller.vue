<script>

export default {
  name: 'Bestseller',
  
}
</script>

<template>

<div class="container-main">
  <div class="fp">
    <div class="sectionTitle d-flex">
      <div class="stripe"></div>
      <h2><strong>Best Seller</strong></h2>
      <div class="stripe"></div>
    </div>
    <p>Must have products from our top sellers</p>
  </div>
  
  <div class="swiper d-flex ">
    <div class="arrow left"><i class="fa-solid fa-chevron-left"></i></div>
    <ul>
      <li>
        <img src="../../assets/spring_printed_dress-400x520.jpg" alt="">
      </li>
      <li>
        <img src="../../assets/modern_love_tee-400x520.jpg" alt="">
      </li>
      <li>
        <img src="../../assets/black_leather_jacket-400x520.jpg" alt="">
      </li>
      <li>
        <img src="../../assets/black_elegant_leather_jacket-400x520.jpg" alt="">
      </li>
      <li>
        <img src="../../assets/hipster_black_top-400x520.jpg" alt="">
      </li>
    </ul>
    <div class="arrow right"><i class="fa-solid fa-chevron-right"></i></div>
  </div>
</div>

</template>

<style lang="scss" scoped>

.fp {
  padding-top: 50px;
  text-align: center;
  p {
    
    padding: 20px 0;
  }
}
.swiper {
  width: 100%;
  ul {
    display: flex;
    list-style: none;
    width: 100%;
    li {
      width: 100%;
      padding: 10px;
      img {
        width: 100%;
        height: 300px;
      }
    }
  }
}


</style>