<template>

  <section class="corporate-weddings">
    <h5 class="title-section">CORPORATE & WEDDINGS</h5>
    <h2 class="title-2">Baking Special Moments</h2>

    <div class="cw-image-box">
      <img class="cw-image" src="../assets/img/corporate-bg.jpg" alt="">
      <img class="cw-image" src="../assets/img/wedding-bg.jpg" alt="">
    </div>
  </section>
  
</template>

<script>
export default {
  name: 'CorporateWeddings'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.corporate-weddings{
  margin-bottom: 200px;

  .title-section, .title-2{
    text-align: center;
  }

  .cw-image-box{
    display: flex;
    justify-content: space-between;

    .cw-image{
      width: 800px;
    }
  }
}

</style>