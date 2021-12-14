<template>

  <div>

    <main class="container">
      <OurProduct />
      <CorporateWeddings />
      <Carousel />
      <BakeryProcess />
      <Locations />
      <Social />
    </main>

    <CallToAction />

  </div>
  
</template>

<script>

import OurProduct from './OurProduct.vue';
import CorporateWeddings from './CorporateWeddings.vue';
import Carousel from './Carousel.vue';
import BakeryProcess from './BakeryProcess.vue';
import Locations from './Locations.vue';
import Social from './Social.vue';
import CallToAction from './CallToAction.vue';


export default {
  name: 'Main',
  components: {
    OurProduct,
    CorporateWeddings,
    Carousel,
    BakeryProcess,
    Locations,
    Social,
    CallToAction,
  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

</style>