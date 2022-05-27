<template>
  <div>

    <HeaderComp />
    <TestimonialsComp />
    <SpecialsComp />
    <BuildComp />
    <FlavorsComp />
    <DealsComp />
    <ReserveComp />
    <FooterComp />

  </div>
</template>

<script>
import HeaderComp from './components/HeaderComp.vue'
import TestimonialsComp from './components/TestimonialsComp.vue'
import SpecialsComp from './components/SpecialsComp.vue'
import BuildComp from './components/BuildComp.vue'
import FlavorsComp from './components/FlavorsComp.vue'
import DealsComp from './components/DealsComp.vue'
import ReserveComp from './components/ReserveComp.vue'
import FooterComp from './components/FooterComp.vue'

export default {
  name: 'App',
  components: {
    HeaderComp,
    TestimonialsComp,
    SpecialsComp,
    BuildComp,
    FlavorsComp,
    DealsComp,
    ReserveComp,
    FooterComp
  }
}
</script>

<style lang="scss">

</style>
