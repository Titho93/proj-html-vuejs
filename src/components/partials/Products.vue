<script>

export default {
  name: 'Products',
  data () {
    return {
        cards: [
            {
                men: [
                    {
                        image: 'black_elegant_leather_jacket-400x520.jpg',
                        font: 'fa-regular fa-square-check',
                        title: 'Black Leather Jacket',
                        bio: 'Men,Jackets,Jeans',
                        discount: '$235',
                        price: '$200'
        
                    },
                    {
                        image: 'black_leather_suit-400x520.jpg',
                        font: 'fa-regular fa-square-check',
                        title: 'Black Leather Suit',
                        bio: 'Men,Jackets',
                        price: '$176'
        
                    },
                    {
                        image: 'blue_jacket_and_white_stripe_tee-400x520.jpg',
                        font: 'fa-regular fa-square-check',
                        title: 'Blue Jacket & Stripe Tee',
                        bio: 'Men,Jackets,Suits',
                        price: '$580'
        
                    },
                    {
                        image: 'modern_black_leather_suit-400x520.jpg',
                        font: 'fa-regular fa-square-check',
                        title: 'Modern Black Leather Suit',
                        bio: 'Men,Jackets',
                        price: '$96'
        
                    }
    
                ],
                women: [
                    {
                        image: 'spring_printed_dress-400x520.jpg',
                        font: 'fa-regular fa-square-check',
                        title: 'Spring Printed Dress',
                        bio: 'Women,Dress',
                        price: '$47'
                    },
                    {
                        image: 'modern_love_tee-400x520.jpg',
                        font: 'fa-regular fa-square-check',
                        title: 'Modern Love Tee',
                        bio: 'Women,T-Shirt',
                        price: '$68'
                    },
                    {
                        image: 'black_leather_jacket-400x520.jpg',
                        font: 'fa-regular fa-square-check',
                        title: 'Black Leather Jacket',
                        bio: 'Women,Jacket,Leather',
                        price: '$125'
                    },
                    {
                        image: 'hipster_black_top-400x520.jpg',
                        font: 'fa-regular fa-square-check',
                        title: 'Hipster Black Top',
                        bio: 'Women,Top',
                        price: '$57'
                    }
                ],
                accessories: [
                    {
                        image: 'leather_gloves-400x520.jpg',
                        font: 'fa-regular fa-square-check',
                        title: 'Leather Gloves',
                        bio: 'Unisex,Gloves',
                        price: '$45',
                       
                    },
                    {
                        image: 'modern_leather_boots-400x520.jpg',
                        font: 'fa-regular fa-square-check',
                        title: 'Modern Leather Boots',
                        bio: 'Man,Boots',
                        discount: '$50',
                        price: '$30',
                    }
                ],
            }
        ],
        selectedCategory: [],
    }
  },
  methods: {
    showCategory(category) {
        this.selectedCategory = this.cards[0][category];
    }
  }
}
</script>

<template>
  
    <div class="container-main">

        <div class="fp">
            <div class="sectionTitle d-flex">
                <div class="stripe"></div>
                <h2><strong>Featured Products</strong></h2>
                <div class="stripe"></div>
            </div>
            <p>Must have products from our top sellers</p>
        </div>

        <div class="select">
            <ul>
                <li @click="showCategory('men')">Men</li>
                <li @click="showCategory('women')">Women</li>
                <li @click="showCategory('accessories')">Accessories</li>
            </ul>
        </div>

        <div class="card-product">
            <ul>
                <li v-for="item in selectedCategory"
                :key="item.title">
                    <div class="card-pt">
                        <div class="image">
                            <img :src="`/assets/${ item.image }`" alt="">
                            <div class="hover-card"><i :class="item.font"></i></div>
                        </div>
                        <h4>{{item.title}}</h4>
                        <span class="bio">{{item.bio}}</span>
                        <div class="price">
                            <span class="discount">{{item.discount}}</span>
                            <span class="real">{{item.price}}</span>
                        </div>
                    </div>
                </li>
                
            </ul> 
        </div>

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

.select {

    ul {
        list-style: none;
        display: flex;
        justify-content: center;
        li {
            cursor: pointer;
            padding: 15px 60px;
            border: 1px solid $lightgrey-color;
            background-color: $darkwhite-color;
            &:nth-child(2) {
                border-left: none;
                border-right: none;
            }
        }
    }
}

.card-product {
    padding: 50px 0;
    ul {
        display: flex;
        list-style: none;
        li {
            .card-pt {
                .image {
                    cursor: pointer;
                    position: relative;
                    width: 100%;
                    height: 100%;
                    img {
                        width: 100%;
                    }
                    .hover-card {
                        display: none;
                        width: 90%;
                        height: 100%;
                        top: 0;
                        position: absolute;
                        background: linear-gradient(#5087d4e9 0%, #8692d4e6 25%, rgba(173, 157, 211, 0.913) 50%, #f0a6d2f5 100%);
                        justify-content: center;
                        align-items: center;
                        i {
                            width: 60px;
                            height: 60px;
                            text-align: center;
                            line-height: 60px;
                            font-size: 25px;
                            border-radius: 50%;
                            color: $white-color;
                            background-color: $low-black;
                        }
                    }
                }
                h4 {
                    padding-top: 20px;
                }
                span {
                    font-size: 12px;
                }
                .price {
                    display: flex;
                    color: $blue-color;
                    padding-top: 10px;
                    span {
                        padding-right: 5px;
                        font-size: 15px;
                    }
                    .discount {
                        font-size: 12px;
                        line-height: 25px;
                    }
                }
            }
            
        }
    }
}

</style>