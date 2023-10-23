<script>

export default {
  name: 'Bestseller',
  data () {
    return {
      cards: [
        {
          image: 'spring_printed_dress-400x520.jpg',
          title: 'Spring Printed Dress',
          text: 'Women,Dress',
          price: '$47'
        },
        {
          image: 'modern_love_tee-400x520.jpg',
          title: 'Modern Love Tee',
          text: 'Women,T-Shirt',
          price: '$68'
        },
        {
          image: 'black_leather_jacket-400x520.jpg',
          title: 'Black Leather Jacket',
          text: 'Women,Jacket,Leather',
          price: '$125'
        },
        {
          image: 'black_elegant_leather_jacket-400x520.jpg',
          title: 'Black Elegant Leather Jacket',
          text: 'Man,Jacket,Leather',
          price: '$200'
        },
        {
          image: 'hipster_black_top-400x520.jpg',
          title: 'Hipster Black Top',
          text: 'Women,Top',
          price: '$57'
        },
        {
          image: 'black_leather_suit-400x520.jpg',
          title: 'Black Leather Suit',
          text: 'Men,Jackets',
          price: '$176'
        },
        {
          image: 'blue_jacket_and_white_stripe_tee-400x520.jpg',
          title: 'Blue Jacket & Stripe Tee',
          text: 'Men,Jackets,Suits',
          price: '$580'
        },
        {
          image: 'modern_black_leather_suit-400x520.jpg',
          title: 'Modern Black Leather Suit',
          text: 'Men,Jackets',
          price: '$96'
        },
        {
          image: 'leather_gloves-400x520.jpg',         
          title: 'Leather Gloves',
          text: 'Unisex,Gloves',
          price: '$45',       
        },
        {
          image: 'modern_leather_boots-400x520.jpg',
          title: 'Modern Leather Boots',
          text: 'Man,Boots',
          price: '$30',
        }        
      ],
      current: 0,
      maxItems: 5,
    }
  },
  computed: {
    visibleCards() {
      return this.cards.slice(this.current, this.current + this.maxItems);
    }
  },
  methods: {
  showNext() {
    if (this.current + this.maxItems < this.cards.length) {
      this.current += this.maxItems;
    } else {
      this.current = 0
    }
  },
},
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
    <div @click="showNext" class="arrow left"><i class="fa-solid fa-chevron-left"></i></div>

    <ul>
      <li v-for="(card,index) in visibleCards"
      :key="index">
        <img :src="`../../assets/${card.image}`" alt="">
        <div class="hover-li">
          <div class="back">
            <div class="bio">
              <h4>{{card.title}}</h4>
              <p>{{ card.text }}</p>
              <span>{{ card.price  }}</span>
            </div>
            <div class="menu">
              <span class="cart"><i class="fa-solid fa-cart-shopping"></i> Add to cart</span>
              <span class="details"><i class="fa-solid fa-list-ul"></i> Details</span>
            </div>
          </div>
        </div>
      </li>
    </ul>

    <div @click="showNext" class="arrow right"><i class="fa-solid fa-chevron-right"></i></div>
  </div>
</div>

</template>

<style lang="scss" scoped>

@use '../../scss/partials/Font.scss' as *;
@use '../../scss/partials/Var.scss' as *;
@use '../../scss/partials/Hover.scss' as *;

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
      img {
        width: 100%;
      }
      .hover-li {
        display: none;
        width: 90%;
        height: 100%;
        top: 0;
        position: absolute;
        background: linear-gradient(#5087d4e9 0%, #8692d4e6 25%, rgba(173, 157, 211, 0.913) 50%, #f0a6d2f5 100%);
        color: $white-color;
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
            }
            .details {
              position: absolute;
              right: 20px;
              bottom: 20px;
            }
          }
        }
      }
    }
  }
}


</style>