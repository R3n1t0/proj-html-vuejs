<template>
  <div class="specials container-fluid rl-container py-2">
    <div class="row rl-row">
      <div class="left col-6 d-flex justify-content-center align-items-center">
        <img src="../assets/img/h1-img-7n.png" alt="img-7">
      </div>

      <div class="col-5 right">
        <div class="text">
          <div class="title pb-3">
            <h1>SPECIALS *</h1>
            <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Distinctio esse voluptas facilis</p>
          </div>
          <div class="combos">
            <div class="combo-p d-flex py-2">
              <h3 class="red">$10</h3>
              <div class="combo ms-3">
                <h3>COMBO PICCOLO</h3>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Distinctio esse voluptas facilis</p>
              </div>
            </div>
            <div class="combo-m d-flex py-2">
              <h3 class="red">$10</h3>
              <div class="combo ms-3">
                <h3>COMBO MEZZO</h3>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Distinctio esse voluptas facilis</p>
              </div>
            </div>
            <div class="combo-g d-flex py-2">
              <h3 class="red">$10</h3>
              <div class="combo ms-3">
                <h3>COMBO GRANDE</h3>
                <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Distinctio esse voluptas facilis</p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "SpecialsComp"
}
</script>

<style lang="scss" scoped>
.rl-container{
  height: 740px;
  .rl-row{
    height: 100%;
    .left{
      height: 100%;
      background-image: url("../assets/img/h1-img-4.jpg");
      background-size: cover;
      background-position: center;
      background-position: 50% 50%;
    }

    .right{
      padding: 110px 130px;
      text{
        width: 60%;
      }

      .red{
        color: #ab4027;
      }
          
      p{
        color: #767676;
      }
    } 
  }  
}

</style>