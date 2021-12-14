<template>

  <main class="container">

    <OurProduct />
    <CorporateWeddings />
    <Carousel />
    <BakeryProcess />
    <Locations />

  </main>
  
</template>

<script>

import OurProduct from './OurProduct.vue';
import CorporateWeddings from './CorporateWeddings.vue';
import Carousel from './Carousel.vue';
import BakeryProcess from './BakeryProcess.vue';
import Locations from './Locations.vue';

export default {
  name: 'Main',
  components: {
    OurProduct,
    CorporateWeddings,
    Carousel,
    BakeryProcess,
    Locations
  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

</style>