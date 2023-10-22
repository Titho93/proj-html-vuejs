<script>

export default {
  name: 'Repilogue',
  data () {
    return {
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
            }
        ],    
        list: [
            'Aenean lobortis sapien enim viverra',
            'Duis ac massa semper maximus',
            'Nunc fermint nulla eu justo sem id',
            'Aliquam posuere magna eget nibh',
            'Cras ac nulla ac consencte rutrum',
            'Fusce mattis nunc ut aliquam'
        ],
        tags: [
            'Black','Boots','Brown','Casual','D&G','Fabric','flowers','Grey','Hat','Hipster','lines','multi-purpose',
            'New-York','Outdoors','red','responsive','summer','sweater','Travel','Warm','White','winter'
        ]
    }
  }
}

</script>

<template>

    <div class="container-se">
        <div class="repilogue d-flex">

            <div class="contacts">
                <img src="../../assets/classic_shop_logo_footer.png" alt="">
                <div class="contact d-flex">
                    <span>12345 North Main Street,</span>
                    <span>New York,NY 555555</span>
                    <span>Phone:1.800.555.6789</span>
                    <span>Email:info@company.com</span>
                    <span>Web: Theme-fusion.com</span>
                </div>
                <div class="social">
                    <ul>
                    <li><i class="fa-brands fa-facebook-f"></i></li>
                    <li><i class="fa-brands fa-twitter"></i></li>
                    <li><i class="fa-brands fa-instagram"></i></li>
                    <li><i class="fa-brands fa-youtube"></i></li>
                    </ul>
                </div>
            </div>
            <div class="replist d-flex">
                <ul class="rated">
                    <span class="title">TOP RATED PRODUCTS</span>
                    <li v-for="(product,index) in products" class="d-flex"
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
                <ul class="post">
                    <span class="title">RECENT POSTS</span>
                    <li v-for="(item,index) in list"
                    :key="index">
                        <span><i class="fa-solid fa-chevron-right"></i>{{ item }}</span>
                    </li>
                </ul>
                <ul class="tags">
                    <span class="title">TAGS</span>
                    <li>
                        <span v-for="(tag,index) in tags" 
                        :key="index"
                        class="tag">{{ tag }}</span>
                    </li>    
                </ul>
            </div>

        </div>

    </div>


</template>

<style lang="scss" scoped>

.container-se {
    background-color: #2B2E32;
    width: 100%;
    height: 480px;
    .repilogue {
        width: 70%;
        margin: 0 auto;
        .contacts {
            padding-top: 70px;
            img {
                height: 40px;
            }
            .contact {
                padding: 50px 0;
                flex-direction: column;
                color: white;
                font-size: 14px;
                span {
                    padding: 5px 0 ;
                }
            }
            .social {
                ul {
                    display: flex;
                    margin-left: -30px;
                    list-style: none;
                    li {
                        cursor: pointer;
                        color: white;
                        padding-right: 15px;
                        &:hover {
                            color: #427ED1;
                        }
                    }
                }
            }
        }
        .replist {
            width: 100%;
            padding-top: 50px;
            padding-left: 80px;
            ul {
                list-style: none;
                color: white;
                width: 100%;
                .title {
                    font-size: 12px;
                    display: inline-block;
                    padding-bottom: 20px;
                }
                li {
                    cursor: pointer;
                    padding: 10px 0;
                    border-bottom: 1px solid #F5F5F5;
                    .bio {
                        width: 205px;
                        flex-direction: column;
                        .object {
                            font-size: 14px;
                            &:hover {
                                color: #427ED1;
                            }
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
            .post {
                li {
                    cursor: pointer;
                    font-size: 14px;
                    :hover {
                        color: #427ED1;
                    }
                    i {
                        font-size: 12px;
                        padding: 8px;
                    }
                }
            }
            .tags {
                li {
                    border-bottom: none;
                    padding: 0;
                    :hover {
                        color: #427ED1;
                    }
                }
            }
        }
    }
}

</style>