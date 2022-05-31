<template>

  <div class="testimonial rl-container">

    <div class="container-fluid">
      <div class="row py-2">
        <div class="col-3 rl-col pe-2">
          <img  src="../assets/img/h3-img-1.jpg" alt="img-1">
          <div class="back">
            <span><i class="fa-regular fa-eye"></i></span>
          </div>
        </div>
        <div class="col-3 rl-col pe-2">
          <img src="../assets/img/h3-img-2.jpg" alt="img-2">
          <div class="back">
            <span><i class="fa-regular fa-eye"></i></span>
          </div>
        </div> 
        <div class="col-3 rl-col pe-2">
          <img src="../assets/img/h3-img-3.jpg" alt="img-3">
          <div class="back">
            <span><i class="fa-regular fa-eye"></i></span>
          </div>
        </div>
        <div class="col-3 rl-col ">
          <img src="../assets/img/h3-img-4.jpg" alt="img-4">
          <div class="back">
            <span><i class="fa-regular fa-eye"></i></span>
          </div>
        </div>
      </div>
    </div>

    <div class="testimonials d-flex justify-content-center align-items-center">
      <button class="prev d-flex justify-content-center align-items-end pb-1">PREV</button>
      <div class="next d-flex justify-content-center align-items-end pb-1">NEXT</div>
      <img src="../assets/img/h3-testimonials-bckgrnd.jpg" alt="">
      <div class="posts">
        <span>“</span>
        <div class="washington">
          <h3>
            “Forget the trendy pizza shops, This hidden spot makes the best New York-style pizza slice in naples”
          </h3>
          <p>Washington Post 2018</p>
        </div>
      </div>
    </div>

  </div>
  
</template>

<script>
export default {
  name: "TestimonialsComp",
  data(){
    return{
      hover: false
    }
  }
}
</script>

<style lang="scss" scoped>
.rl-container{
  width: 100%;
  .rl-col{
    position: relative;
    padding: 0;
    img{
      width: 100%;
      height: 100%;
      &:hover{
        display: none;
      }
    }

    .back{
      display: none;
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background-color: white;

      span{
        position: relative;
        width: 100px;
        height: 100px;
        border-radius: 50%;
        background-color: #d2401e;
        i{
          font-size: 20px;
          position: absolute;
          top: 42%;
          left: 40%;
          color: white;
        }
      }
    }
  }

  .testimonials{
  position: relative;
  width: 100%;
  height: 480px;
  span{
    /* font-size: 150px; */
    color: #b68a2c;
  }

  img{
    width: 100%;
    height: 100%;
  }

  .prev, .next{
    position: absolute;
    width: 80px;
    height: 40px;
    border: none;
    border-top-left-radius: 40px;
    border-top-right-radius: 40px;
    background-color: white;
    color: #d2401e;
    border: none;
  }

  .prev{
    transform: rotate(90deg);
    left: -20px;
    bottom: 50%;
  }
  .next{
    transform: rotate(-90deg);
    right: -20px;
    bottom: 50%;
  }

  .posts{
    width: 60%;
    position: absolute;
    margin-left: auto;
    margin-right: auto;
    left: 0;
    right: 0;
    text-align: center;
    .washington{
       p{
      color: #d2401e;
      }
      h3{
        font-size: 35px;
      }
    }
  }
}

}



</style>