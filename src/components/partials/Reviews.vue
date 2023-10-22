<script>

export default {
  name: 'Reviews'
}
</script>

<template>
  
  <div class="reviews">
    <div class="backfirst">
        <img src="../../assets/testimonials_home_1_bg.jpg" alt="">
    </div>
    <div class="backsecond">
        <img src="../../assets/testimonials_home_1_bg.jpg" alt="">
    </div>
    <div class="bio">
        <img src="../../assets/man_testimonial.png" alt="">
        <p>Curabitur non tristique tortor. Vestibulum aliquet suscipit ipsum in volupat. Donec vel lacinia sem, vitae semper nulla. In hac habitasse platea dictumst. Mauris consectetur est et nibh sadip hendrerit bibendum.</p>
       <span><strong>Dario Pineda</strong>, Theme Fusion</span>
       <div class="circle">
        <i class="fa-solid fa-circle"></i>
        <i class="fa-regular fa-circle"></i>
       </div>
    </div>

  </div>

</template>

<style lang="scss" scoped>

@use '../../scss/partials/Font.scss' as *;
@use '../../scss/partials/Var.scss' as *;
@use '../../scss/partials/Hover.scss' as *;

.reviews {
    margin-top: 130px;
    width: 100%;
    height: 550px;
    position: relative;
    .backfirst {
        img {
            width: 100%;
            height: 165px;
            object-fit: cover;
        }
    }
    .backsecond {
        img {
            width: 100%;
            height: 385px;
            object-fit: cover;
        }
    }
    .bio {
        text-align: center;
        position: absolute;
        color: $white-color;
        top: 21%;
        left: 28%;
        p {
            width: 850px;
            font-size: 18px;
            padding: 25px 0;
        }
        span {
            font-size: 20px;
        }
        .circle {
            i {
                padding: 30px 5px;
                font-size: 12px;
            }
        }
    }
}

</style>