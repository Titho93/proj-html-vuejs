<script>

export default {
  name: 'Headerbottom',
  
}
</script>

<template>
  
  <div class="container-bt">

    <div class="nav-bottom">
      
      <div class="logo">
        <img src="../../assets/classic_shop_logo1x.png" alt="">
      </div>
      <div class="menu">
        <ul>
          <li>Home <i class="fa-solid fa-chevron-down"></i></li>
          <li>Shop <i class="fa-solid fa-chevron-down"></i></li>
          <li>Products <i class="fa-solid fa-chevron-down"></i></li>
          <li>Categories <i class="fa-solid fa-chevron-down"></i></li>
          <li>News</li>
          <li>Elements <i class="fa-solid fa-chevron-down"></i></li>
        </ul>
        <button>SHOP NOW!</button>
        <span><i class="fa-solid fa-magnifying-glass"></i></span>
      </div>

    </div>

  </div>

</template>

<style lang="scss">

.container-bt {
  width: 70%;
  margin: 0 auto;
}

.nav-bottom {
  width: 100%;
  height: 100px;
  display: flex;
  .logo {
    padding: 30px 40px;
  }
  .menu {
    display: flex;
    ul {
      display: flex;
      list-style: none;
      li {
        font-size: 15px;
        margin-left: 40px;
        line-height: 100px;
        cursor: pointer;
        &:hover {
          border-top: 2px solid #427ED1;
          color: #427ED1;
        }
        i {
          font-size: 10px;
          padding: 0 5px;
        }
      }
    }
    button {
      height: 40px;
      padding: 0 30px;
      background-color: #427ED1;
      color: white;
      border-radius: 20px;
      font-size: 13px;
      border: none;
      margin: 32px;
      &:hover {
        opacity: 50%;
      }
    }

    span {
      i {
        line-height: 100px;
        font-size: 13px;
      }
    }

  }
}



</style>