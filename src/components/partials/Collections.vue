<script>

export default {
  name: 'Collections',

  
}
</script>

<template>

    <div class="collection">
        <div class="square">
            <div class="image">
                <img src="../../assets/winter_collection_bg.jpg" alt="">
            </div>
            <div class="bios">
                <h2>Winter Collection</h2>
                <p>STYLISH AND WARM</p>
                <button>VIEW MORE</button>
            </div>
        </div>
        <div class="square">
            <div class="image">
                <img src="../../assets/spring_collection_bg.jpg" alt="">
            </div>
            <div class="bios">
                <h2>Spring Collectionn</h2>
                <p>BRIGHT AND COLORFUL</p>
                <button>VIEW MORE</button>
            </div>
        </div>
        <div class="square">
            <div class="image">
                <img src="../../assets/autumn_collection_bg.jpg" alt="">
            </div>
            <div class="bios">
                <h2>Autumn Collection</h2>
                <p>RICH AND CONFORTABLE</p>
                <button>VIEW MORE</button>
            </div>
        </div>
    </div>
  
  

</template>

<style lang="scss">

.collection {
    padding-top: 150px;
    display: flex;
    width: 100vw;
    .square {
        color: white;
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
            button {
                padding: 10px 25px;
                font-size: 13px;
            }
        }
    }
}

</style>