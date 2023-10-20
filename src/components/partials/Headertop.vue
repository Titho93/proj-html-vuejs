<script>

export default {
  name: 'Headertop',
  data () {
    return {
      iconsocial: [
      {
        href: '#',
        font: 'fa-brands fa-facebook-f'
      },
      {
        href: '#',
        font: 'fa-brands fa-twitter'
      },
      {
        href: '#',
        font: 'fa-brands fa-instagram'
      },
      {
        href: '#',
        font: 'fa-brands fa-youtube'
      }
      ] 
    }
  }
  
}
</script>

<template>
  
  <div class="container-bt">
    
    <div class="nav">
      
      <div class="social">
        <ul>
          <li v-for="(item,index) in iconsocial"
          :key="index">
            <a :href="item.href">
              <i :class="item.font"></i>
            </a>
          </li>
        </ul>
      </div>
  
      <div class="menu-list">
        <ul>
          <li>Shopping Cart</li>
          <li>My Account <i class="fa-solid fa-chevron-down small"></i></li>
          <li class="cart"><i class="fa-solid fa-cart-shopping"></i> CART <i class="fa-solid fa-chevron-down"></i></li>
        </ul>
      </div>
    </div>
  </div>  


  
</template>

<style lang="scss" scoped>

.container-bt {
  width: 70%;
  margin: 0 auto;
}
.nav {
  height: 50px;
  display: flex;
  .social {
    width: 50%;
    display: flex;
    justify-content: start;
    ul {
      li {
        cursor: pointer;
        padding: 12px 10px;
        a{
          color: black;
          &:hover {
            color: #427ED1;
          }
        }
      }
    }
  }
  .menu-list {
    display: flex;
    justify-content: end;
    width: 50%;
    ul {
      font-size: 13px;
      color: #AAAAAA;
      li {
        cursor: pointer;
        border-right: 1px solid #F5F5F5;
        &:hover {
          color: #427ED1;
          background-color: #FAFAFA;
        }
      }
    }
  }
}

.cart {
  color: #494949;
  padding: 15px 50px;
  background-color: FAFAFA;
}

ul {
    list-style: none;
    display: flex;
}

li {
  padding: 15px 10px;
}

</style>