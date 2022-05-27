<template>
  <div class="jumbo-card">
    <div @click="prevSlide()" class="prev"></div>
    
    <img class="front" :src="slides[counterSlide].front" alt="Crust">
    <img class="back" :src="slides[counterSlide].back" alt="Crust">

    <div @click="nextSlide()" class="next"></div>
  </div>
</template>

<script>
export default {
  name: "JumboComp",

  data(){
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
  },

  mounted(){
    this.startAutoScroll();
    this.changeImage(); 
  }
}

</script>

<style lang="scss" scoped> 
.jumbo-card{
  position: relative;
  .front{
    position: absolute;
    top: 50%;
    left: 50%;
    margin-top: -270px; /* Half the height */
    margin-left: -180px;
  }
}

</style>