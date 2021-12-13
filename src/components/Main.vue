<template>

  <main class="container">

    <OurProduct />
    <CorporateWeddings />
    <Carousel />
    <BakeryProcess />

  </main>
  
</template>

<script>

import OurProduct from './OurProduct.vue';
import CorporateWeddings from './CorporateWeddings.vue';
import Carousel from './Carousel.vue';
import BakeryProcess from './BakeryProcess.vue';

export default {
  name: 'Main',
  components: {
    OurProduct,
    CorporateWeddings,
    Carousel,
    BakeryProcess
  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

</style>