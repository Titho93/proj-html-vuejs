<script>

export default {
  name: 'Ourblog',
  data () {
    return {
        squares: [
            {
                image: 'post_img_12-700x441.jpg',
                title: 'Aenean lobortis sapien enim viverra',
                date: 'September 9th,2015',
                comments: '0 Comments',
                text: 'Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla.'
            },
            {
                image: 'post_img_11-700x441.jpg',
                title: 'Duis ac massa semper maximus',
                date: 'September 9th,2015',
                comments: '0 Comments',
                text: 'Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla.'
            },
            {
                image: 'post_img_10-700x441.jpg',
                title: 'Nunc fermint nulla eu justo sem id',
                date: 'September 9th,2015',
                comments: '0 Comments',
                text: 'Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla.'
            },
        ]
    }
  }
  
}
</script>

<template>
  
    <div class="container-main">
        <div class="fp">
            <div class="sectionTitle d-flex">
            <div class="stripe"></div>
            <h2><strong>From Our Blog</strong></h2>
            <div class="stripe"></div>
            </div>
            <p>The latest Classic Shop news</p>
        </div>

        <div class="squares d-flex">
            <div v-for="(square,index) in squares" class="square"
            :key="index">
                <img :src="`../../assets/${ square.image }`" alt="">
                <h4><strong>{{ square.title }}</strong></h4>
                <span>{{ square.date }} | {{ square. comments}}</span>
                <p> {{ square.text }}</p>
            </div>
        </div>
    </div>

</template>

<style lang="scss" scoped>
.container-main {
    padding-top: 120px;
}
.fp {
    text-align: center;
    p {
        padding-top: 20px;
    }
}
.squares {
    padding-top: 50px;
    .square {
        margin: 0 auto;
        height: 230px;
        &:nth-child(2) {
            padding: 0 30px;
        }
        img {
            width: 100%;
        }
        h4 {
            font-size: 18px;
            padding-top: 18px;
        }
        span {
            font-size: 14px;
        }
        p {
            font-size: 16px;
            padding: 15px 0;
        }
    }
}
</style>