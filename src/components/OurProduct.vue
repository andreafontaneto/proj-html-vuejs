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


    <div class="product-image-box">
      <div class="l-product-image">
        <img src="../assets/img/choco-chip-cookies.jpg" alt="">
      </div>

      <div class="r-product-image">
        <img src="../assets/img/strawberry-jam-cookies.jpg" alt="">
      </div>

      <div class="l-arrow"><i class="fas fa-chevron-left"></i></div>
      <div class="r-arrow"><i class="fas fa-chevron-right"></i></div>
    </div>

  </section>
  
</template>

<script>
export default {
  name: 'OurProduct'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.product{
  height: 700px;
  display: flex;
  justify-content: space-between;

  .product-inner{
    width: 30%;

    .product-text{
      width: 100%;

      .btn{
        width: 170px;
        padding: 15px 0;
      }
    }
  }

  .product-image-box{
    width: 65%;
    height: 100%;
    display: flex;
    position: relative;

    .l-product-image, .r-product-image{
      width: 50%;
      padding: 10px;

      img{
        width: 600px;
      }
    }

    .l-arrow, .r-arrow{
      width: 50px;
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