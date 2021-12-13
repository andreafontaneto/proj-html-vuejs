<template>

  <main class="container">

    <OurProduct />
    <CorporateWeddings />

  </main>
  
</template>

<script>

import OurProduct from './OurProduct.vue';
import CorporateWeddings from './CorporateWeddings.vue';

export default {
  name: 'Main',
  components: {
    OurProduct,
    CorporateWeddings
  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

</style>