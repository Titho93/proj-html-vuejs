<script>

export default {
  name: 'Jumbotron',
  
}
</script>

<template>

  <div class="container-jb">

    <img src="/home1_slide_three_bg_2.jpg" alt="">

    <div class="description">

      <h1>Brand New Arrivals</h1>
      <h4>NEW COLLECTION FROM NEW YORK</h4>

      <div class="buttons">
        <button>VIEW ALL</button>
        <button>LOOKBOOK</button>
      </div>

    </div>

  </div>
  
</template>

<style lang="scss">

@use '../scss/Main.scss';

.container-jb {
  width: 100vw;
  height: 650px;
  position: relative;
  img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .description {
    position: absolute;
    width: 100%;
    top: 185px;
    text-align: center;
    .buttons {
      padding-top: 20px;
      button {
        margin: 8px;
      }
    }
  }
  h4 {
    color: white;
  }
}
</style>