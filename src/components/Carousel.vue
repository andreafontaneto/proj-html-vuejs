<template>
  <section class="carousel">
    <div class="carousel-inner">
      <h2 class="title-2">Find a freshly baked product perfect for you</h2>
      <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Aperiam magnam rem repudiandae sunt cumque et perferendis saepe id velit sint.</p>
      <div class="btn btn-violet">Shop All Products</div>
    </div>

    <div class="carousel-image-box">
      <div class="crsl-item">
        <img src="../assets/img/choco-chip-cookies.jpg" alt="">
        <h3 class="title-3">Choco Chip Cookies</h3>
        <p class="subtitle">$19.00 - $39.00</p>
      </div>
      <div class="crsl-item">
        <img src="../assets/img/strawberry-jam-cookies.jpg" alt="">
        <h3 class="title-3">Strawberry Jam Cookies</h3>
        <p class="subtitle">$19.00 - $39.00</p>
      </div>
      <div class="crsl-item">
        <img src="../assets/img/strawberry-donut.jpg" alt="">
        <h3 class="title-3">Strawberry Donut</h3>
        <p class="subtitle">$19.00 - $39.00</p>
      </div>
      <div class="crsl-item">
        <img src="../assets/img/perfect-macarons.jpg" alt="">
        <h3 class="title-3">Perfect Macaron</h3>
        <p class="subtitle">$19.00 - $39.00</p>
      </div>

      <div class="l-arrow"><i class="fas fa-chevron-left"></i></div>
      <div class="r-arrow"><i class="fas fa-chevron-right"></i></div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Carousel'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.carousel{
  height: 500px;
  margin-bottom: 150px;
  display: flex;
  justify-content: space-between;

  .carousel-inner{
    width: 25%;
    height: 100%;
    text-align: center;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    .title-2{
      margin-bottom: 10px;
    }

    .subtitle{
      margin-bottom: 30px;
    }
  }

  .carousel-image-box{
    width: 70%;
    height: 100%;
    display: flex;
    align-items: flex-end;
    position: relative;

    .crsl-item{
      width: calc(100% / 4 - 20px);
      margin: 0 10px;
      text-align: center;

      .title-3{
        margin: 20px 0 10px 0;
      }

      .subtitle{
        color: $violet-color;
      }
    }

    .l-arrow, .r-arrow{
      width: 40px;
      height: 80px;
      background-color: rgba($violet-color, 0.4);
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      position: absolute;
      transform: translateY(-50%);
    }

    .l-arrow{
      top: 50%;
      left: 10px;
    }

    .r-arrow{
      top: 50%;
      right: 10px;
    }
  }
}

</style>