<template>

  <main class="container">

    <OurProduct />

  </main>
  
</template>

<script>

import OurProduct from './OurProduct.vue'

export default {
  name: 'Main',
  components: {
    OurProduct
  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

</style>