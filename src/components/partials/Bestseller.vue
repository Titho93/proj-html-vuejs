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
        <div class="hover-li">
          <div class="back">
            <div class="bio">
              <h4>Spring Printed Dress</h4>
              <p>Women,Dress</p>
              <span>$47</span>
            </div>
            <div class="menu">
              <span class="cart"><i class="fa-solid fa-cart-shopping"></i> Add to cart</span>
              <span class="details"><i class="fa-solid fa-list-ul"></i> Details</span>
            </div>
          </div>
        </div>
      </li>
      <li>
        <img src="../../assets/modern_love_tee-400x520.jpg" alt="">
        <div class="hover-li">
          <div class="back">
            <div class="bio">
              <h4>Modern Love Tee</h4>
              <p>Women,T-Shirt</p>
              <span>$68</span>
            </div>
            <div class="menu">
              <span class="cart"><i class="fa-solid fa-cart-shopping"></i> Add to cart</span>
              <span class="details"><i class="fa-solid fa-list-ul"></i> Details</span>
            </div>
          </div>
        </div>
      </li>
      <li>
        <img src="../../assets/black_leather_jacket-400x520.jpg" alt="">
        <div class="hover-li">
          <div class="back">
            <div class="bio">
              <h4>Black Leather Jacket</h4>
              <p>Women,Jacket,Leather</p>
              <span>$125</span>
            </div>
            <div class="menu">
              <span class="cart"><i class="fa-solid fa-cart-shopping"></i> Add to cart</span>
              <span class="details"><i class="fa-solid fa-list-ul"></i> Details</span>
            </div>
          </div>
        </div>
      </li>
      <li>
        <img src="../../assets/black_elegant_leather_jacket-400x520.jpg" alt="">
        <div class="hover-li">
          <div class="back">
            <div class="bio">
              <h4>Black Elegant Leather Jacket</h4>
              <p>Man,Jacket,Leather</p>
              <span>$200</span>
            </div>
            <div class="menu">
              <span class="cart"><i class="fa-solid fa-cart-shopping"></i> Add to cart</span>
              <span class="details"><i class="fa-solid fa-list-ul"></i> Details</span>
            </div>
          </div>
        </div>
      </li>
      <li>
        <img src="../../assets/hipster_black_top-400x520.jpg" alt="">
        <div class="hover-li">
          <div class="back">
            <div class="bio">
              <h4>Hipster Black Top</h4>
              <p>Women,Top</p>
              <span>$57</span>
            </div>
            <div class="menu">
              <span class="cart"><i class="fa-solid fa-cart-shopping"></i> Add to cart</span>
              <span class="details"><i class="fa-solid fa-list-ul"></i> Details</span>
            </div>
          </div>
        </div>
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
      position: relative;
      cursor: pointer;
      &:hover {
        .hover-li {
          display: block;
        }
      }
      img {
        width: 100%;
        height: 300px;
      }
      .hover-li {
        display: none;
        width: 90%;
        height: 100%;
        top: 0;
        position: absolute;
        background: linear-gradient(#5087d4e9 0%, #8692d4e6 25%, rgba(173, 157, 211, 0.913) 50%, #f0a6d2f5 100%);
        color: white;
        text-align: center;
        justify-content: center;
        align-items: center;
        .back {
          height: 100%;
          width: 100%;
          .bio {
            height: 100%;
            width: 100%;
            display: flex;
            flex-direction: column;
            justify-content: center;
            h4 {
              font-size: 15px;
            }
            p {
              font-size: 12px;
            }
            
          }
          .menu {
            font-size: 12px;
            position: relative;
            .cart {
              position: absolute;
              left: 20px;
              bottom: 20px;
              &:hover {
                color: #427ED1;
              }
            }
            .details {
              position: absolute;
              right: 20px;
              bottom: 20px;
              &:hover {
                color: #427ED1;
              }
            }
          }
        }
      }
    }
  }
}


</style>