<script>

export default {
  name: 'Payment'
}

</script>

<template>

<div class="container-se">
    <div class="pay d-flex">
        <span>Copyright 2012 - 2020 | Avada Theme by Theme Fusion | All Rights Reserved | Powered by WordPress</span>
        <ul>
            <li>
                <a href="#">
                    <img src="../../assets/visa.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../../assets/paypal.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../../assets/mastercard.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../../assets/discover.png" alt="">
                </a>
            </li>
            <li>
                <a href="#">
                    <img src="../../assets/amazon.png" alt="">
                </a>
            </li>
        </ul>

    </div>
</div>

  
</template>

<style lang="scss" scoped>

.container-se {
    width: 100%;
    height: 120px;
    background-color: #1C1E21;
    .pay {
        padding-top: 40px;
        flex-direction: column;
        text-align: center;
        span {
            color: white;
            font-size: 12px;

        }
        ul {
            list-style: none;
            display: flex;
            justify-content: center;
            li {
                margin: 10px 5px;
                img {
                    width: 50px;
                }
            }
        }
    }    
}



</style>