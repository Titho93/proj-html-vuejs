<script>



export default {
  name: 'Send'
  
}

</script>

<template>

<div class="container-se">
  <div class="send d-flex">
    <div class="subscrive d-flex">
      <i class="fa-regular fa-envelope"></i>
      <h3>Subscrive now and get special offers</h3>
    </div>
    <div class="mail">
      <input type="text" placeholder="Insert your email">
      <button class="blue">SEND</button>
    </div>  


  </div>

</div>
  
</template>

<style lang="scss" scoped>

@use '../../scss/partials/Font.scss' as *;
@use '../../scss/partials/Var.scss' as *;
@use '../../scss/partials/Hover.scss' as *;

.container-se {
  height: 230px;
  background-color: $dark-grey;
  .send {
    text-align: center;
    margin: 0 auto;
    width: 70%;
    height: 100%;
    .subscrive {
      height: 90%;
      padding: 80px 0;
      i {
        width: 60px;
        height: 60px;
        font-size: 35px;
        border-radius: 50%;
        background-color: $light-black;
        color: $lightgrey-color;
        line-height: 60px;
      }
      h3 {
        line-height: 60px;
        color: $white-color;
        font-size: 35px;
        padding: 0 30px;
      }
    }  
    .mail {
      padding: 60px 0;
      input {
        font-size: 12px;
        padding: 10px 20px;
        border-radius: 20px;
        width: 285px;
        border: none;
        margin-left: 100px;
      }
      button {
        padding: 10px 50px;
      }
    }
  }
}

</style>