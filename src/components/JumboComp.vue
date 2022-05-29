<template>
  <div class="jumbo-card d-flex justify-content-center">
    <button class="prev d-flex justify-content-center align-items-end pb-1">PREV</button>
    <img src="../assets/img/h3-rev-img-1.png" alt="">
    <img class="first" src="../assets/img/h3-rev-img-2.png" alt="">
    <div class="next d-flex justify-content-center align-items-end pb-1">NEXT</div>
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
  width: 100%;
  position: relative;
  .first{
    position: absolute;
    margin-left: auto;
    margin-right: auto;
    left: 0;
    right: 0;
    text-align: center;
  }
  .prev, .next{
    position: absolute;
    width: 80px;
    height: 40px;
    border: none;
    border-top-left-radius: 40px;
    border-top-right-radius: 40px;
    background-color: #f7f7f2;
    color: #d2401e;
  }

  .prev{
    transform: rotate(90deg);
    left: -30px;
    bottom: 50%;
  }
  .next{
    transform: rotate(-90deg);
    right: -30px;
    bottom: 50%;
  }
}



</style>