<script>

export default {
  name: 'Headertop',
  
}
</script>

<template>
  
    
    <div class="nav">
      
      <div class="social">
        <ul>
          <li><i class="fa-brands fa-facebook-f"></i></li>
          <li><i class="fa-brands fa-twitter"></i></li>
          <li><i class="fa-brands fa-instagram"></i></li>
          <li><i class="fa-brands fa-youtube"></i></li>
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



  
</template>

<style lang="scss" scoped>

.nav {
  display: flex;
  .social {
    flex-grow: 3;
    ul {
      li {
        padding: 10px;
      }
    }
  }
  .menu-list {
    flex-grow: 1;
    ul {
      font-size: 13px;
      color: #AAAAAA;
      li {
        padding: 10px;
        border-right: 1px solid #AAAAAA;
      }
    }
  }
}

ul {
    list-style: none;
    display: flex;
}

</style>