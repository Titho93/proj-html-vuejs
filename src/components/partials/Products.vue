<script>

export default {
  name: 'Products',
  data () {
    return {
        cards: [
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
                <h2><strong>Featured Products</strong></h2>
                <div class="stripe"></div>
            </div>
            <p>Must have products from our top sellers</p>
        </div>

        <div class="select">
            <ul>
                <li>Men</li>
                <li>Women</li>
                <li>Accessories</li>
            </ul>
        </div>

        <div class="card-product">
            <ul>
                <li v-for="(card,index) in cards"
                :key="index">
                    <div class="card-pt">
                        <div class="image">
                            <img :src="`/assets/${ card.image }`" alt="">
                            <div class="hover-card"><i :class="card.font"></i></div>
                        </div>
                        <h4>{{card.title}}</h4>
                        <span class="bio">{{card.bio}}</span>
                        <div class="price">
                            <span class="discount">{{card.discount}}</span>
                            <span class="real">{{card.price}}</span>
                        </div>
                    </div>
                </li>
                
            </ul> 
        </div>

    </div>

</template>

<style lang="scss" scoped>

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
            border: 1px solid #AAAAAA;
            background-color: #F5F5F5;
            &:nth-child(2) {
                border-left: none;
                border-right: none;
            }
            &:hover {
                background-color: white;
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
                    &:hover {
                        .hover-card {
                            display: flex;
                        }
                    }
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
                            color: white;
                            background-color: #2B2E32;
                            &:hover {
                                background-color: #e4e6e9;
                                color: black;
                            }
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
                    color: #427ED1;
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