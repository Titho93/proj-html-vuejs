<script>

export default {
  name: 'Headerbottom',
  data () {
    return {
      list: [
        {
          text: 'Home',
          font: 'fa-solid fa-chevron-down'
        },
        {
          text: 'Shop',
          font: 'fa-solid fa-chevron-down'
        },
        {
          text: 'Products',
          font: 'fa-solid fa-chevron-down'
        },
        {
          text: 'Categories',
          font: 'fa-solid fa-chevron-down'
        },
        {
          text: 'News',
        },
        {
          text: 'Elements',
          font: 'fa-solid fa-chevron-down'
        }
      ]
    }
  }
  
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
          <li v-for="(item,index) in list"
          :key="index">{{item.text}} 
          <i :class="item.font"></i>
          </li>
        </ul>
        <button class="blue">SHOP NOW!</button>
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
    width: 30%;
  }
  .menu {
    display: flex;
    ul {
      display: flex;
      list-style: none;
      li {
        font-size: 13px;
        margin-left: 40px;
        line-height: 100px;
        border-top: 3px solid white;
        cursor: pointer;
        &:hover {
          border-top: 3px solid #427ED1;
          color: #427ED1;
        }
        i {
          font-size: 10px;
          padding: 0 5px;
        }
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