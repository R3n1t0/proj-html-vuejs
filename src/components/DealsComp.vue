<template>
  <div class="deals d-flex">
    <div class="left">
      <div class="title pb-4">
        <p>MADE WITH LOVE</p>
        <h2> DELISH PIZZA DEALS</h2>
      </div>
      <div class="dates mt-3">
        <div class="date d-flex">
          <div class="day pe-5">
            <h2>02</h2>
            <h4>NOV</h4>
          </div>
          <div class="location">
            <h4>TRADITIONAL NEAPOLITAN PIES IN KYOTO PIZZA MERCATO</h4>
            <p><i class="fa-solid fa-location-dot"></i> 204 E.Pizzetta Tommaso</p>
          </div>
        </div>
        <div class="dots">
        </div>
      </div>
      <div class="dates mt-3">
        <div class="date d-flex">
          <div class="day pe-5">
            <h2>03</h2>
            <h4>NOV</h4>
          </div>
          <div class="location">
            <h4>TRADITIONAL NEAPOLITAN PIES IN KYOTO PIZZA MERCATO</h4>
            <p><i class="fa-solid fa-location-dot"></i> 204 E.Pizzetta Tommaso</p>
          </div>
        </div>
        <div class="dots">
        </div>
      </div>
      <div class="dates mt-3">
        <div class="date d-flex">
          <div class="day pe-5">
            <h2>05</h2>
            <h4>NOV</h4>
          </div>
          <div class="location">
            <h4>TRADITIONAL NEAPOLITAN PIES IN KYOTO PIZZA MERCATO</h4>
            <p><i class="fa-solid fa-location-dot"></i> 204 E.Pizzetta Tommaso</p>
          </div>
        </div>
        <div class="dots">
        </div>
      </div>
    </div>

    <div class="right">
    </div>
  </div>

</template>

<script>
export default {
  name: "DealsComp"
}
</script>

<style lang="scss" scoped>
.deals{
  width: 100%;
  height: 750px;
  color: white;
  .left, .right{
    width: 50%;
    height: 100%;
    background-image: url("../assets/img/header-background.jpg");
    background-size: cover;
    background-position: center;
    padding: 80px 110px;
    p{
      color: #d2401e;
      font-size: 12px;
    }
    .day{
      h2{
        color: #ab4027;
      }
    }

    .dots{
      border-color: #b7903c;
      border-bottom-style: dotted;
      margin: 30px 0;
    }

  }
  .right{ 
    background-image: url("../assets/img/h3-img-5a.jpg");
  }
}

</style>