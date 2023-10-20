<script>

export default {
  name: 'Offer',
}
</script>

<template>

    <div class="offer">
        <div class="squares d-flex">
            <div class="square">
                <img src="../../assets/promo_box_1_bg.jpg" alt="">
                <div class="bio">
                    <h2>70% Off</h2>
                    <p>Vivamus tempor leo lacus, feugiat ut magna aliquam erat.</p>
                    <button class="small">VIEW MORE</button>
                </div>
            </div>
            <div class="square">
                <img src="../../assets/promo_box_2_bg.jpg" alt="">
                <div class="bio">
                    <h2>Free Shipping</h2>
                    <p>Vivamus tempor leo lacus, feugiat ut magna aliquam erat.</p>
                    <button class="small">VIEW MORE</button>
                </div>
            </div>
        </div>
    </div>
    

</template>

<style lang="scss" scoped>

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
                color: white;
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