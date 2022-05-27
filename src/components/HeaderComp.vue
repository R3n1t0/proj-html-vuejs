<template>
  <header class="container-fluid">
    <div class="top container d-flex justify-content-center align-items-center pt-3">
      <div class="left d-flex justify-content-between align-items-center">
        <a>ORDER ONLINE</a>

        <nav>
          <ul class="d-flex align-items-center mb-0">
            <img src="../assets/svg/svg-0.svg" alt="">
            <li>HOME</li>
            <li>PAGES</li>
            <li>MENU</li>
          </ul>
        </nav>
      </div>

      <div class="center d-flex align-items-center m-4">
        <img src="../assets/img/h5-logo-divided-header.png" alt="">
      </div>

      <div class="right d-flex justify-content-between">
        <nav>
          <ul class="d-flex mb-0 px-0">
            <li>EVENT</li>
            <li>BLOG</li>
            <li>LANDING</li>
          </ul>
        </nav>

        <div class="search-cart">
          <img src="../assets/svg/svg-1.svg" alt="">
          <a href="#">CART</a>
          <i class="fa-solid fa-magnifying-glass mx-2"></i>
          <a href="#">SEARCH</a>
        </div>
      </div>
    </div>

    <div class="bottom">
      <JumboComp />
    </div>
  </header>
</template>

<script>
import JumboComp from './JumboComp.vue'

export default {
  name: "HeaderComp",
  components:{
    JumboComp
  }
}
</script>

<style lang="scss" scoped>
header{
  height: 700px;
  background-image: url("../assets/img/header-background.jpg");
  color: #ffffff;
  font-size: 12px;
  font-weight: 500;
  text-transform: uppercase;
  .top{
    height: 150px;
    .left{
      width: 40%;
      a{
        background-color: #d2401e;
        padding: 15px 30px;
      }
      img{
        width: 30px;
        height: 10px;
        margin: 3px;
        fill: #ffffff;
      }
      li{
        margin-right: 30px;
      }
    } 

    .center{
      height: 100%;
      img{
        height: 85%;
      }
    }

    .right{
      width: 40%;
      li{
        margin-left: 30px;
      }

      .search-cart{
        a{
          text-decoration: none;
          color: #ffffff;
        }
      }
    }
  }

  .bottom{
    width: 100%;
    height: calc(100% - 150px);
  }
}

</style>