<template>
  <div class="jumbo-card d-flex justify-content-center">
    <img src="../assets/img/h3-rev-img-1.png" alt="">
    <img class="first" src="../assets/img/h3-rev-img-2.png" alt="">
  </div>
 
</template>

<script>
export default {
  name: "JumboComp",
}

/*   data(){
    return{
      slides:[
        {
          front: "../assets/img/h3-rev-img-2.png",
          back: "../assets/img/h3-rev-img-1.png"
        },
        {
          front: "../assets/img/h3-rev-img-4.png",
          back: "../assets/img/h3-rev-img-3.png"
        },
        {
          front: "../assets/img/h3-rev-img-6.png",
          back: "../assets/img/h3-rev-img-5.png"
        }
      ],

      counterSlide: 0,

      autoScroll: null
    
    }
  */

/*   mounted(){
    this.startAutoScroll();
    this.changeImage(); 
  },

  methods: {
    nextSlide(){
      this.counterSlide ++;
      if (this.counterSlide > this.slides.length - 1){
        this.counterSlide = 0;
      }
    },
    prevSlide(){
      this.counterSlide --;
      if (this.counterSlide < 0){
        this.counterSlide = this.slides.length -1;
      }
    },
    changeImage(index){        
      this.counterSlide = index;
    },
    mouseOver(){
      clearInterval(this.autoScroll);
      this.autoScroll = null;         
    },
    mouseOut(){    
      this.startAutoScroll();
    },
    startAutoScroll(){
      this.autoScroll = setInterval(() =>{
        this.nextSlide();
      },3000)
    }
  }
} */

</script>

<style lang="scss" scoped> 
.jumbo-card{
  position: relative;
  .first{
    position: absolute;
    margin-left: auto;
    margin-right: auto;
    left: 0;
    right: 0;
    text-align: center;
  }
}



</style>