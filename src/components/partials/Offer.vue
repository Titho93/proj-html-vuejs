<script>

export default {
  name: 'Offer',
  data () {
    return {
        squares: [
            {
                image: 'promo_box_1_bg.jpg',
                title: '70% Off',
                text: 'Vivamus tempor leo lacus, feugiat ut magna aliquam erat.'
            },
            {
                image: 'promo_box_2_bg.jpg',
                title: 'Free Shipping',
                text: 'Vivamus tempor leo lacus, feugiat ut magna aliquam erat.'
            },
        ]
    }
  }
}
</script>

<template>

    <div class="offer">
        <div class="squares d-flex">
            <div v-for="(square,index) in squares" class="square"
            :key="index">
                <img :src="`../../assets/${square.image}`" alt="">
                <div class="bio">
                    <h2>{{ square.title }}</h2>
                    <p>{{ square.text }}</p>
                    <button class="small">VIEW MORE</button>
                </div>
            </div>
        </div>
    </div>
    

</template>

<style lang="scss" scoped>

@use '../../scss/partials/Font.scss' as *;
@use '../../scss/partials/Var.scss' as *;
@use '../../scss/partials/Hover.scss' as *;

.offer {
    margin-top: 100px;
    width: 100%;
    height: 550px;
    background-image: url(../../assets/bkgd_confetti-compressor.jpg);
    background-position: center;
    .squares {
        width: 70%;
        height: 100%;
        margin: 0 auto;
        justify-content: center;
        .square {
            display: flex;
            align-items: center;
            padding: 20px;
            position: relative;
            img {
                width: 100%;
                height: 370px;
            }
            .bio {
                color: $white-color;
                position: absolute;
                top: 35%;
                left: 15%;
                h2 {
                    font-size: 45px;
                }
                p {
                    width: 250px;
                    font-size: 15px;
                }
            }
        }
    }
}

</style>