<script>

export default {
  name: 'Repilogue'
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
                    <li class="d-flex">
                        <div class="bio d-flex">
                            <span class="object">Leather Gloves</span>
                            <span class="stars">
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                            </span>
                            <div class="price">
                                <span class="real">$45</span>
                            </div>
                        </div>
                        <img src="../../assets/leather_gloves-400x520.jpg" alt="">
                    </li>
                    <li class="d-flex">
                        <div class="bio d-flex">
                            <span class="object">Black Leather Jacket</span>
                            <span class="stars">
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                            </span>
                            <div class="price">
                                <span class="discount">$235</span>
                                <span class="real">$200</span>
                            </div>
                        </div>
                        <img src="../../assets/black_elegant_leather_jacket-400x520.jpg" alt="">
                    </li>
                    <li class="d-flex">
                        <div class="bio d-flex">
                            <span class="object">Spring Printed Dress</span>
                            <span class="stars">
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                                <i class="fa-solid fa-star"></i>
                            </span>
                            <div class="price">
                                <span class="real">$47</span>
                            </div>
                        </div>
                        <img src="../../assets/spring_printed_dress-400x520.jpg" alt="">
                    </li>

                </ul>
                <ul class="post">
                    <span class="title">RECENT POSTS</span>
                    <li>
                        <span><i class="fa-solid fa-chevron-right"></i>Aenean lobortis sapien enim viverra</span>
                    </li>
                    <li>
                        <span><i class="fa-solid fa-chevron-right"></i>Duis ac massa semper maximus</span>
                    </li>
                    <li>
                        <span><i class="fa-solid fa-chevron-right"></i>Nunc fermint nulla eu justo sem id</span>
                    </li>
                    <li>
                        <span><i class="fa-solid fa-chevron-right"></i>Aliquam posuere magna eget nibh</span>
                    </li>
                    <li>
                        <span><i class="fa-solid fa-chevron-right"></i>Cras ac nulla ac consencte rutrum</span>
                    </li>
                    <li>
                        <span><i class="fa-solid fa-chevron-right"></i>Fusce mattis nunc ut aliquam</span>
                    </li>
                </ul>
                <ul class="tags">
                    <span class="title">TAGS</span>
                    <li>
                        <span class="tag">Black</span>
                        <span class="tag">Boots</span>
                        <span class="tag">Brown</span>
                        <span class="tag">Casual</span>
                    </li>
                    <li>
                        <span class="tag">D&G</span>
                        <span class="tag">Fabric</span>
                        <span class="tag">flowers</span>
                        <span class="tag">Grey</span>
                    </li>
                    <li>
                        <span class="tag">Hat</span>
                        <span class="tag">Hipster</span>
                        <span class="tag">lines</span>
                    </li>
                    <li>
                        <span class="tag">multi-purpose</span>
                        <span class="tag">New York</span>
                    </li>
                    <li>
                        <span class="tag">Outdoors</span>
                        <span class="tag">red</span>
                        <span class="tag">responsive</span>
                    </li>
                    <li>
                        <span class="tag">summer</span>
                        <span class="tag">sweater</span>
                        <span class="tag">Travel</span>
                    </li>
                    <li>
                        <span class="tag">Warm</span>
                        <span class="tag">White</span>
                        <span class="tag">winter</span>
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