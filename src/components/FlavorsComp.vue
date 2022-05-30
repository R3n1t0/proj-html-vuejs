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
          <img :src = "require(`../assets/img/h3-product-img-${pizza.src}.png`)" :alt="pizza.name">
          <p class="pt-3 pb-0">{{pizza.name}}</p>
          <span>{{pizza.price}}</span>
        </div>
        
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
          src: "1a-100x100",
          price: "$55.00",
          name: "CAMPAGNOLA"
        },
        {
          src: "2a-150x150",
          price: "$7.00 - $55.00",
          name: "FIORI DI ZUCCA"
        },
        {
          src: "3a-150x150",
          price: "$30.00",
          name: "FRANCESCANA"
        },
        {
          src: "4a-150x150",
          price: "$45.00",
          name: "VALDOSTANA"
        },
        {
          src: "5a-150x150",
          price: "$25.00 - $55.00",
          name: "TARTUFATA"
        },
        {
          src: "6a-100x100",
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
        width: 80%;
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