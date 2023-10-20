<script>

export default {
  name: 'Brand'
}
</script>

<template>
  
  <div class="container-lo">
      <span>BRAND LOGOS</span>
      <div class="logos">
        <ul>
            <li>
                <img src="../../assets/b_logotype_6.png" alt="">
            </li>
            <li>
                <img src="../../assets/b_logotype_7.png" alt="">
            </li>
            <li>
                <img src="../../assets/b_logotype_1.png" alt="">
            </li>
            <li>
                <img src="../../assets/b_logotype_2.png" alt="">
            </li>
            <li>
                <img src="../../assets/b_logotype_3.png" alt="">
            </li>
        </ul>
    </div>

  </div>
 

</template>

<style lang="scss" scoped>

.container-lo {
    width: 100%;
    height: 300px;
    padding-top: 60px;
    text-align: center;
    background-color: #F5F5F5;
    span {
        letter-spacing: 0.2em;
        padding-left: 30px;
    }
    .logos {
        padding-top: 40px;
        margin: 0 auto;
        width: 70%;
        ul {
            display: flex;
            list-style: none;
            li {
                width: 100%;
            }
        }
    }
}


</style>