<template>
  <div class="container-fluid rl-container">
    <div class="text">
      <h1>
        GO AHEAD AND BUILD YOUR OWN PIZZA WE WON’T JUDGE!
      </h1>
    </div>

  </div>
</template>

<script>
export default {
  name: "BuildComp"
}
</script>

<style lang="scss" scoped>
.rl-container{
  position: relative;
  height: 500px;
  background-image: url("../assets/img/h3-background-img.jpg");
  background-size: cover;
  background-position: center;
  background-position: 50% 50%;
  .text{
    position: absolute;
    width: 20%;
    font-weight: bold;
    color: white;
    top: 120px;
    left: 150px;
  }
}

</style>