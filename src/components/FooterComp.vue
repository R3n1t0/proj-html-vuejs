<template>
  <footer class="d-flex">
    <div class="left row">

      <div class="our-res col-4">
        <h5>FIND OUR RESTAURANTS</h5>
        <div class="salento py-3">
          <p>1614 E. Bell Rd #104.</p>
          <p>Salerno, AZ 85022</p>
          <p>(602) 867-1010</p>
        </div>
        <div class="sorrento pb-3">
          <p>204 E. Pizzetta Tommaso</p>
          <p>Sorrento, AZ 85022</p>
          <p>(358) 867-1010</p>
        </div>
        <div class="torre pb-3">
          <p>Vale Puglia 54</p>
          <p>Torre Del Greco AZ 85022</p>
          <p>(359) 867-1010</p>
        </div>
        <div class="naples pb-3">
          <p>Corso Itali AA</p>
          <p>Naples, AZ 85022</p>
          <p>(989) 867-1010</p>
        </div>
      </div>

      <div class="working-hours col-4">
        <h5>WORKING HOURS</h5>
        <div class="monday py-3">
          <h6>MONDAY</h6>
          <span>Kitchen Closed</span>
        </div>
        <div class="friday pb-3">
          <h6>TUSEDAY UNTIL FRIDAY</h6>
          <p>9:00 - 22:00</p>
        </div>
        <div class="saturday pb-3">
          <h6>SATURDAY <span>*</span></h6>
          <p>Saturday 11am to midnight</p>
        </div>
        <div class="sunday pb-3">
          <h6>SUNDAY</h6>
          <p>9:00 - 22:00</p>
        </div>
        <div class="follow py-3">
          <h6>FOLLOW US:
            <i class="fa-brands fa-twitter"></i>
            <i class="fa-brands fa-facebook-f"></i>
            <i class="fa-brands fa-instagram-square"></i>
            <i class="fa-brands fa-linkedin-in"></i>
          </h6>
        </div>
      </div>

      <div class="crew col-4">
        <h3>
          THE DON PEPPE CREW FIRST AND FOREMOST VALUES AN AUTHENTIC, WELL BAKED SLICE OF PIZZA
        </h3>
      </div>


    </div>

    <div class="right">
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComp"
}
</script>

<style lang="scss" scoped>
footer{
  width: 100%;
  height: 700px;
  color: white;
  .left{
    padding: 130px 65px;
    background-image: url("../assets/img/header-background.jpg");
    h5, h6{
      color: #b68a2c;
    }
    h6{
      margin-bottom: 0;
    }
    p{
      margin-bottom: 5px;
      color: #a6a6a6;
    }
    span{
      color: #d2401e;
    }

    .follow{
      i{
        color: white;
        font-size: 12px;
        padding-left: 10px;
      }
    }
  }
  .right{
    background-image: url("../assets/img/footer-img-1.jpg");
  }
  .left, .right{
    width: 50%;
    height: 100%;
    background-size: cover;
    background-position: center;
  }
}

</style>