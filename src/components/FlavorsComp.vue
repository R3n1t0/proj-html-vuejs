<template>
  <div class="flavors d-flex justify-content-center align-items-center flex-column">
    <div class="best d-flex justify-content-center align-items-center flex-column py-5">  
      <span class="red">CHOOSE YOURE FLAVOR</span>
      <h1 class="pb-2">THE BEST PIZZA IN TOWN</h1>
      <p>
        Lorem ipsum dolor, sit amet consectetur adipisicing elit. Iusto, laudantium hic earum illo natus maiores? Sed aut libero omnis qui!
      </p> 
    </div>

    <div class="pizza-slider">
      <div class="pizza-types d-flex justify-content-between">

        <div 
          v-for="(pizza, index) in pizzas"
          :key="index"
          class="pizza-card d-flex justify-content-center align-items-center flex-column">
          <img :src=pizza.src :alt="pizza.name">
          <p>{{pizza.name}}</p>
          <span>{{pizza.price}}</span>
        </div>
<!--         <div class="pizza-card d-flex justify-content-center align-items-center flex-column">
          <img src="../assets/img/h3-product-img-2a-150x150.png" alt="product-2">
          <p>FIORI DI ZUCCA</p>
          <span>$7.00 - $50.00</span>
        </div>
        <div class="pizza-card d-flex justify-content-center align-items-center flex-column">
          <img src="../assets/img/h3-product-img-3a-150x150.png" alt="product-3">
          <p>FIORI DI ZUCCA</p>
          <span>$7.00 - $50.00</span>
        </div>
        <div class="pizza-card d-flex justify-content-center align-items-center flex-column">
          <img src="../assets/img/h3-product-img-4a-150x150.png" alt="product-4">
          <p>FIORI DI ZUCCA</p>
          <span>$7.00 - $50.00</span>
        </div>
        <div class="pizza-card d-flex justify-content-center align-items-center flex-column">
          <img src="../assets/img/h3-product-img-5a-150x150.png" alt="product-5">
          <p>FIORI DI ZUCCA</p>
          <span>$7.00 - $50.00</span>
        </div>
        <div class="pizza-card d-flex justify-content-center align-items-center flex-column">
          <img src="../assets/img/h3-product-img-6a-100x100.png" alt="product-6">
          <p>FIORI DI ZUCCA</p>
          <span>$7.00 - $50.00</span>
        </div>  -->
        
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "FlavorsComp",

  data(){
    return{
      pizzas:[
        {
          src: "../assets/img/h3-product-img-1a-100x100.png",
          price: "$55.00",
          name: "CAMPAGNOLA"
        },
        {
          src: "../assets/img/h3-product-img-2a-150x150.png",
          price: "$7.00 - $55.00",
          name: "FIORI DI ZUCCA"
        },
        {
          src: "../assets/img/h3-product-img-3a-150x150.png",
          price: "$30.00",
          name: "FRANCESCANA"
        },
        {
          src: "../assets/img/h3-product-img-4a-150x150.png",
          price: "$45.00",
          name: "VALDOSTANA"
        },
        {
          src: "../assets/img/h3-product-img51a-150x150.png",
          price: "$25.00",
          name: "TARTUFATA"
        },
        {
          src: "../assets/img/h3-product-img-6a-100x100.png",
          price: "$15.00",
          name: "BISMARCK"
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.best{
  width: 40%;
  text-align: center;
  .red{
    color: #ab4027;
    font-size: 12px;
  }
  p{
    color: #767676;
  }
}

.pizza-slider{
  width: 100%;
  .pizza-types{
    width: 100%;
    .pizza-card{
      width: calc(100% / 5);
      img{
        width: 70%;
      }
      p{
        color: #b68a2c;
      }
      span{
        color: #d2401e;
      }
    }
  }
}

</style>