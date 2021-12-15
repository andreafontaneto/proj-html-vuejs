<template>

  <section class="corporate-weddings">
    <h5 class="title-section">CORPORATE & WEDDINGS</h5>
    <h2 class="title-2">Baking Special Moments</h2>

    <div class="cw-image-box">

      <div class="cw-image-left">
        <img class="cw-image" src="../assets/img/corporate-bg.jpg" alt="">
        <img class="cw-image-hover" src="../assets/img/corporate-hover-bg.jpg" alt="">
      </div>
      <div class="cw-image-right">
        <img class="cw-image" src="../assets/img/wedding-bg.jpg" alt="">
        <img class="cw-image-hover" src="../assets/img/wedding-hover-bg.jpg" alt="">
      </div>

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

    .cw-image-left, .cw-image-right{
      width: 50%;
      height: 850px;
      position: relative;

      .cw-image, .cw-image-hover{
        position: absolute;
        top: 0;
        left: 0;
      }

      .cw-image{
        display: block;
      }

      .cw-image-hover{
        display: none;
      }

      .cw-image:hover{
        display: none;
      }

      .cw-image:hover .cw-image-hover{
        display: block;
      }

    }

    .cw-image-left{
      margin-right: 40px;
    }

    .cw-image-right{
      margin-left: 40px;
    }
    
  }
}

</style>