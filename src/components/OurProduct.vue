<template>

  <section class="product">

    <div class="product-inner">
      <div class="product-text">
        <h5 class="title-section">OUR PRODUCTS</h5>
        <h2 class="title-2">All our delectable pastries are backed fresh in our Kitchen very morning, and are made with all-natural, all organic ingredients.</h2>
          
        <div class="btn btn-violet">
          <span>Start Shopping</span>
        </div>
      </div>
    </div>

    <Slider2Items />

  </section>
  
</template>

<script>

import Slider2Items from './Slider2Items.vue';

export default {
  name: 'OurProduct',
  components: {
    Slider2Items
  }

}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.product{
  height: 700px;
  display: flex;
  justify-content: space-between;
  margin-bottom: 150px;

  .product-inner{
    width: 30%;

    .product-text{
      width: 100%;
    }
  }

}


</style>