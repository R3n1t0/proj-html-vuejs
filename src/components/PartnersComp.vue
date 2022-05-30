<template>
  <div class="partners container-fluid p-0">
    
    <div class="rl-container">
      <div class="row py-2 me-0">
        <div class="col-3 p-0">
          <img src="../assets/img/h1-team-1a-700x700.jpg" alt="team-1">
        </div>
        <div class="col-3 p-0">
          <img src="../assets/img/h1-team-2a.jpg" alt="team-2">
        </div>
        <div class="col-3 p-0">
          <img src="../assets/img/h1-team-3a.jpg" alt="team-3">
        </div>
        <div class="col-3 p-0">
          <img src="../assets/img/h1-team-4a.jpg" alt="team-4">
        </div>
      </div>
    </div>

    <div class="clients p-5 d-flex justify-content-center align-items-center">
      <img src="../assets/img/h1-clients-img-1.png" alt="clients-1">
      <img src="../assets/img/h1-clients-img-2.png" alt="clients-2">
      <img src="../assets/img/h1-clients-img-3.png" alt="clients-3">
      <img src="../assets/img/h1-clients-img-4.png" alt="clients-4">
    </div>

  </div>
</template>

<script>
export default {
  name: "PartnersComp"
}
</script>

<style lang="scss" scoped>
.rl-container{
  width: 100%;
  .row{
    img{
      width: 100%; 
    }
  }
 
}

.clients{
  background-color: #f7f7f2;
  img{
    width: 17%;
  }
}


</style>