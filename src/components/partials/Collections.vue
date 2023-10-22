<script>

export default {
  name: 'Collections',
  data () {
    return {
        squares: [
            {
                image: 'winter_collection_bg.jpg',
                title: 'Winter Collection',
                bio: 'STYLISH AND WARM'
            },
            {
                image: 'spring_collection_bg.jpg',
                title: 'Spring Collectionn',
                bio: 'BRIGHT AND COLORFUL'
            },
            {
                image: 'autumn_collection_bg.jpg',
                title: 'Autumn Collection',
                bio: 'RICH AND CONFORTABLE'
            }
        ]
    }
  }
}
</script>

<template>

    <div class="collection">
        <div v-for="(square,index) in squares" class="square"
        :key="index">
            <div class="image">
                <img :src="`../../assets/${square.image}`" alt="">
            </div>
            <div class="bios">
                <h2>{{square.title}}</h2>
                <p>{{square.bio}}</p>
                <button class="small">VIEW MORE</button>
            </div>
        </div>
    </div>
  
  

</template>

<style lang="scss" scoped>

@use '../../scss/partials/Font.scss' as *;
@use '../../scss/partials/Var.scss' as *;
@use '../../scss/partials/Hover.scss' as *;

.collection {
    padding-top: 150px;
    display: flex;
    width: 100vw;
    .square {
        color: $white-color;
        width: 100%;
        height: 600px;
        position: relative;
        .image {
            width: 100%;
            height: 100%;
            img {
                width: 100%;
                height: 100%;
                object-fit: cover;
                object-position: top;
            }
        }
        .bios {
            position: absolute;
            bottom: 10%;
            left: 25%;
            text-align: center;
            p {
                padding: 10px 0;
                font-size: 20px;
            }
        }
    }
}

</style>