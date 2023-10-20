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
                        <div class="image">
                            <img src="../../assets/black_elegant_leather_jacket-400x520.jpg" alt="">
                            <div class="hover-card"><i class="fa-regular fa-square-check"></i></div>
                        </div>
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
                        <div class="image">
                            <img src="../../assets/black_leather_suit-400x520.jpg" alt="">
                            <div class="hover-card"><i class="fa-regular fa-square-check"></i></div>
                        </div>
                        <h4>Black Leather Suit</h4>
                        <span class="bio">Men,Jackets</span>
                        <div class="price">
                            <span class="real">$176</span>
                        </div>
                    </div>
                </li>
                <li>
                    <div class="card-pt">
                        <div class="image">
                            <img src="../../assets/blue_jacket_and_white_stripe_tee-400x520.jpg" alt="">
                            <div class="hover-card"><i class="fa-regular fa-square-check"></i></div>
                        </div>
                        <h4>Blue Jacket & Stripe Tee</h4>
                        <span class="bio">Men,Jackets,Suits</span>
                        <div class="price">
                            <span class="real">$580</span>
                        </div>
                    </div>
                </li>
                <li>
                    <div class="card-pt">
                        <div class="image">
                            <img src="../../assets/modern_black_leather_suit-400x520.jpg" alt="">
                            <div class="hover-card"><i class="fa-regular fa-square-check"></i></div>
                        </div>
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