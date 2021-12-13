<template>

  <main class="container">

    <OurProduct />
    <CorporateWeddings />
    <Carousel />

  </main>
  
</template>

<script>

import OurProduct from './OurProduct.vue';
import CorporateWeddings from './CorporateWeddings.vue';
import Carousel from './Carousel.vue';

export default {
  name: 'Main',
  components: {
    OurProduct,
    CorporateWeddings,
    Carousel
  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

</style>