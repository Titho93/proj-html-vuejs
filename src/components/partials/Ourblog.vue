<script>

export default {
  name: 'Ourblog'
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
            <div class="square">
                <img src="../../assets/post_img_12-700x441.jpg" alt="">
                <h4><strong>Aenean lobortis sapien enim viverra</strong></h4>
                <span>September 9th,2015 | 0 Comments</span>
                <p>Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla.</p>
            </div>
            <div class="square">
                <img src="../../assets/post_img_11-700x441.jpg" alt="">
                <h4><strong>Duis ac massa semper maximus</strong></h4>
                <span>September 9th,2015 | 0 Comments</span>
                <p>Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla.</p>
            </div>
            <div class="square">
                <img src="../../assets/post_img_10-700x441.jpg" alt="">
                <h4><strong>Nunc fermint nulla eu justo sem id</strong></h4>
                <span>September 9th,2015 | 0 Comments</span>
                <p>Donec finibus sit amet orci eget ultricies. Praesent posuere ante ut erat fringilla.</p>
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