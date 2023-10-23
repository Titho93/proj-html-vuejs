<script>

export default {
  name: 'Reviews',
  data () {
        return {
            firstTestimonials: [
                {
                    image: 'man_testimonial.png',
                    reviews: 'Curabitur non tristique tortor. Vestibulum aliquet suscipit ipsum in volupat. Donec vel lacinia sem, vitae semper nulla. In hac habitasse platea dictumst. Mauris consectetur est et nibh sadip hendrerit bibendum.',
                    name: 'Dario Pineda',
                    position: 'Theme Fusion',
                    circle: 'fa-solid fa-circle',
                    circle2: 'fa-regular fa-circle'
                }
            ],
            secondTestimonials: [    
                {
                    image: 'woman_testimonial.png',
                    reviews: 'Curabitur non tristique tortor. Vestibulum aliquet suscipit ipsum in volupat. Donec vel lacinia sem, vitae semper nulla. In hac habitasse platea dictumst. Mauris consectetur est et nibh sadip hendrerit bibendum.',
                    name: 'Gaia Gomes',
                    position: 'Engineer',
                    circle: 'fa-regular fa-circle',
                    circle2: 'fa-solid fa-circle'
                }
            ],
            showFirst: true
        }
    },
    methods: {
        toggleTestimonials() {
            this.showFirst = !this.showFirst;
        },
    },
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
    <div v-for="testimonial in (showFirst ? firstTestimonials : secondTestimonials)" class="bio"
    :key="testimonial.name">
        <img :src="`../../assets/${testimonial.image}`" alt="">
        <p>{{ testimonial.reviews }}</p>
       <span><strong>{{ testimonial.name }}</strong>, {{ testimonial.position }}</span>
       <div class="circle">
        <i :class="testimonial.circle"
        @click="toggleTestimonials"></i>
        <i :class="testimonial.circle2"
        @click="toggleTestimonials"></i>
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
        position: relative;
        color: $white-color;
        top: -80%;
        p {
            margin: 0 auto;
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