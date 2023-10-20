<script>

export default {
  name: 'Products',
  
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
                <li>
                    <div class="card-pt">
                        <img src="../../assets/black_elegant_leather_jacket-400x520.jpg" alt="">
                        <h4>Black Leather Jacket</h4>
                        <span class="bio">Men,Jackets,Jeans</span>
                        <div class="price">
                            <span class="discount">$235</span>
                            <span class="real">$200</span>
                        </div>
                    </div>
                </li>
                <li>
                    <div class="card-pt">
                        <img src="../../assets/black_leather_suit-400x520.jpg" alt="">
                        <h4>Black Leather Suit</h4>
                        <span class="bio">Men,Jackets</span>
                        <div class="price">
                            <span class="real">$176</span>
                        </div>
                    </div>
                </li>
                <li>
                    <div class="card-pt">
                        <img src="../../assets/blue_jacket_and_white_stripe_tee-400x520.jpg" alt="">
                        <h4>Blue Jacket & Stripe Tee</h4>
                        <span class="bio">Men,Jackets,Suits</span>
                        <div class="price">
                            <span class="real">$580</span>
                        </div>
                    </div>
                </li>
                <li>
                    <div class="card-pt">
                        <img src="../../assets/modern_black_leather_suit-400x520.jpg" alt="">
                        <h4>Modern Black Leather Suit</h4>
                        <span class="bio">Men,Jackets</span>
                        <div class="price">
                            <span class="real">$96</span>
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
                img {
                    width: 80%;
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
                        line-height: 2px;
                    }
                }
            }
            
        }
    }
}

</style>