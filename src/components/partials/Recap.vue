<script>

export default {
  name: 'Recap',
  data () {
    return {
        squares: [
            {
                title: 'FEATURED',
                products: [
                    {
                        title: 'Black Jacket',
                        discount: '',
                        price: '$125',
                        image: 'black_leather_jacket-400x520.jpg'
                    },
                    {
                        title: 'Black Leather Jacket',
                        rate: 'fa-solid fa-star',
                        discount: '$235',
                        price: '$200',
                        image: 'black_elegant_leather_jacket-400x520.jpg'
                    },
                    {
                        title: 'Hipster Black Top',
                        discount: '',
                        price: '$57',
                        image: 'hipster_black_top-400x520.jpg'
                    },
                ]
            },
            {
                title: 'ON SALE',
                products: [
                    {
                        title: 'Black Leather Jacket',
                        rate: 'fa-solid fa-star',
                        discount: '$235',
                        price: '$200',
                        image: 'black_elegant_leather_jacket-400x520.jpg'
                    },
                    {
                        title: 'Blue Leather Jacket',
                        discount: '$80',
                        price: '$60',
                        image: 'blue_leather_jacket-400x520.jpg'
                    },
                    {
                        title: 'Modern Leather Boots',
                        discount: '$50',
                        price: '$30',
                        image: 'modern_leather_boots-400x520.jpg'
                    },
                ]
            },
            {
                title: 'TOP RATED',
                products: [
                    {
                        title: 'Leather Gloves',
                        rate: 'fa-solid fa-star',
                        price: '$45',
                        image: 'leather_gloves-400x520.jpg'
                    },
                    {
                        title: 'Black Leather Jacket',
                        rate: 'fa-solid fa-star',
                        discount: '$235',
                        price: '$200',
                        image: 'black_elegant_leather_jacket-400x520.jpg'
                    },
                    {
                        title: 'Spring Printed Dress',
                        rate: 'fa-solid fa-star',
                        price: '$47',
                        image: 'spring_printed_dress-400x520.jpg'
                    },
                ]
            },
            {
                title: 'LATEST REVIEWS',
                products: [
                    {
                        title: 'Black Leather Jacket',
                        rate: 'fa-solid fa-star',
                        price: 'by admin',
                        image: 'black_elegant_leather_jacket-400x520.jpg'
                    },
                    {
                        title: 'Leather Gloves',
                        rate: 'fa-solid fa-star',
                        price: 'by Beardman',
                        image: 'leather_gloves-400x520.jpg'
                    },
                    {
                        title: 'Spring Printed Dress',
                        rate: 'fa-solid fa-star',
                        price: 'by admin',
                        image: 'spring_printed_dress-400x520.jpg'
                    },
                ]
            }
        ]
    }
  }  
}
</script>

<template>
  <div class="container-rc">
      <div class="recap d-flex">
        <ul v-for="(square,index) in squares"
        :key="index">
            <span class="title">{{ square.title }}</span>
            <li v-for="(product,index) in square.products" class="d-flex"
            :key="index">
                <div class="bio d-flex">
                    <span class="object">{{ product.title }}</span>
                    <span class="stars">
                        <i v-for="index in 5"
                        :key="index"
                        :class="`${ product.rate }`"></i>
                    </span>
                    <div class="price">
                        <span class="discount">{{ product.discount }}</span>
                        <span class="real">{{ product.price }}</span>
                    </div>
                </div>
                <img :src="`../../assets/${ product.image }`" alt="">
            </li>
        </ul>    
 
      </div>

  </div>
  

</template>

<style lang="scss">

@use '../../scss/partials/Font.scss' as *;
@use '../../scss/partials/Var.scss' as *;
@use '../../scss/partials/Hover.scss' as *;

.container-rc {
    margin: 250px auto 0 auto;

    border-top: 2px solid $darkwhite-color;
    width: 98%;

    .recap {
        width: 75%;
        margin: 60px auto;
        ul {
            list-style: none;
            width: 25%;
            .title {
                font-size: 16px;
                letter-spacing: 0.3em;
                display: inline-block;
                padding-bottom: 20px;
            }
            li {
                padding: 10px 0;
                border-bottom: 2px solid $darkwhite-color;
                .bio {
                    width: 205px;
                    flex-direction: column;
                    .object {
                        font-size: 15px;
                    }
                    .price {
                        font-size: 15px;
                        .real {
                            padding-left: 5px;
                        }
                    }
                }
                img {
                    height: 75px;
                }

            }
        }
    }
}

</style>