<template>
  <div class="reserve py-2">
    <div class="inner d-flex justify-content-evenly align-items-center">

      <div class="d-flex justify-content-center align-items-center">

        <div class="info d-flex align-items-center">
          <i class="fa-solid fa-user-group"></i>
          <input type="text" placeholder="1 Person">
        </div>

        <h5>FOR</h5>

        <div class="info d-flex align-items-center">
          <i class="fa-solid fa-calendar"></i>
          <input type="text" placeholder="11/29/2020">
        </div>

        <h5>AT</h5>

        <div class="info d-flex align-items-center">
          <i class="fa-solid fa-clock"></i>
          <input type="text" placeholder="7:00 pm">
        </div>

        <a>BOOK A TABLE</a>

      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: "ReserveComp"
}
</script>

<style lang="scss" scoped>
.inner{
  width: 100%;
  height: 300px;
  background-image: url("../assets/img/h3-background-img-3.jpg");
  background-position: center;
  background-size: cover;
  .info{
    position: relative;
    i{
      position: absolute;
      right: 20px;
      top: 28px;
      color: #b68a2c;
    }
    input{
      width: 250px;
      border: 2px solid black;
      padding: 20px 40px; 
    }
  }
 

  h5{
    color: white;
    margin: 20px;
  }
  
  a{
    margin-left: 70px;
    padding: 20px 80px;
    color: white;
    background-color: #d2401e;
  }
}
</style>