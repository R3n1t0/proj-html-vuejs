<template>
  <div class="container container-fluid">
    <div class="row">
      <div
        v-for="(picture, index) in pictures" 
        :key="index"
        class="co-4">
        <img :src="picture.url" alt="">
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
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>

</style>