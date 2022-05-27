<template>
  <header class="container-fluid">
    <div class="top container d-flex">
      <div class="left d-flex">
        <a>ORDER ONLINE</a>

        <nav>
          <ul class="d-flex">
            <li>HOME</li>
            <li>PAGES</li>
            <li>MENU</li>
          </ul>
        </nav>

      </div>

      <div class="center">
        <img src="../ass" alt="">
      </div>

      <div class="right">

      </div>
    </div>

    <div class="bottom"></div>
  </header>
</template>

<script>
export default {
  name: "HeaderComp"
}
</script>

<style lang="scss" scoped>
header{
  height: 700px;
  background-image: url("../assets/img/header-background.jpg");
  .top{
    height: 150px;
  }
}

</style>