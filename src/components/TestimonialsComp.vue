<template>
  <div class="container-fluid">
    <div class="row py-2">
      <div class="col-3 rl-col ps-0">
        <img src="../assets/img/h3-img-1.jpg" alt="">
      </div>
      <div class="col-3 rl-col ps-0 pe-1">
        <img src="../assets/img/h3-img-2.jpg" alt="">
      </div> 
      <div class="col-3 rl-col pe-0 ps-2">
        <img src="../assets/img/h3-img-3.jpg" alt="">
      </div>
      <div class="col-3 rl-col pe-0">
        <img src="../assets/img/h3-img-4.jpg" alt="">
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TestimonialsComp",

  data(){
    return{
      pictures:[
        {
          url: "../assets/img/h3-img-1.jpg"
        },
        {
          url: "../assets/img/h3-img-2.jpg"
        },
        {
          url: "../assets/img/h3-img-3.jpg"
        },
        {
          url: "../assets/img/h3-img-4.jpg"
        }
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
.rl-col{
  
  img{
    width: 100%;
    height: 100%;
  }
}


</style>