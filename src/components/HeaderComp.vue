<template>
  <header class="container-fluid">
    <div class="top container">
      <TopComp />
    </div>

    <div class="bottom container-fluid-flex justify-content-center pt-3">
      <JumboComp />
    </div>
  </header>
</template>

<script>
import JumboComp from './JumboComp.vue'
import TopComp from './TopComp.vue'

export default {
  name: "HeaderComp",
  components:{
    JumboComp,
    TopComp
  }
}
</script>

<style lang="scss" scoped>
header{
  height: 700px;
  background-image: url("../assets/img/header-background.jpg");
  color: #ffffff;
  font-size: 12px;
  font-weight: 500;
  text-transform: uppercase;
  .top{
    height: 150px;
  }

  .bottom{
    height: calc(100% - 150px);
  }
}

</style>