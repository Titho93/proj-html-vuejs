<script>

export default {
  name: 'Payment',
  data () {
    return {
        paycards: [
            {
                href: '#',
                image: 'visa.png'
            },
            {
                href: '#',
                image: 'paypal.png'
            },    
            {
                href: '#',
                image: 'mastercard.png'
            },
            {
                href: '#',
                image: 'discover.png'
            },
            {
                href: '#',
                image: 'amazon.png'
            }
        ]
    }
  }
}

</script>

<template>

<div class="container-se">
    <div class="pay d-flex">
        <span>Copyright 2012 - 2020 | Avada Theme by Theme Fusion | All Rights Reserved | Powered by WordPress</span>
        <ul>
            <li v-for="(paycard,index) in paycards"
            :key="index">
                <a :href= paycard.href>
                    <img :src="`../../assets/${ paycard.image }`" alt="">
                </a>
            </li>
        </ul>
    </div>
</div>

  
</template>

<style lang="scss" scoped>

.container-se {
    width: 100%;
    height: 130px;
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