<template>
  <div class="top d-flex justify-content-center align-items-center">
    <div class="left d-flex justify-content-between align-items-center">
        <a>ORDER ONLINE</a>

        <nav>
          <ul class="d-flex align-items-center mb-0">
            <img :src="svg0">
            <li>HOME</li>
            <li>PAGES</li>
            <li>MENU</li>
          </ul>
        </nav>
      </div>

      <div class="center d-flex align-items-center m-4">
        <img src="../assets/img/h5-logo-divided-header.png" alt="logo-header">
      </div>

      <div class="right d-flex justify-content-between align-items-center">
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
</template>

<script>

export default {
  name: "TopComp",
  data(){
    return{
      svg0: require("../assets/svg/svg-0.svg")
    }
  }
}
</script>

<style lang="scss" scoped>
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
    color: #ffffff;
  }
  li{
     margin-right: 40px;
  }
} 

.center{
  height: 100%;
  img{
    height: 75%;
  }
}

.right{
  width: 40%;
  li{
    margin-left: 40px;
  }
  .search-cart{
    a{
      text-decoration: none;
      color: #ffffff;
    }
  }
}
</style>