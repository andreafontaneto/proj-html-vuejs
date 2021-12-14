<template>

  <div class="product-image-box">

    <div class="item">
      <img :src="images[counter]" alt="">
    </div>
    <div class="item">
      <img :src="images[counter + 1]" alt="">
    </div>

    <!-- <div class="l-product-image">
      <img src="../assets/img/choco-chip-cookies.jpg" alt="">
    </div>

    <div class="r-product-image">
      <img src="../assets/img/strawberry-jam-cookies.jpg" alt="">
    </div> -->

    <div @click="prevImg" class="l-arrow"><i class="fas fa-chevron-left"></i></div>
    <div @click="nextImg" class="r-arrow"><i class="fas fa-chevron-right"></i></div>

  </div>
  
</template>

<script>
export default {
  name: 'Slider2Items',

  data(){
    return{

      images: [
        require('../assets/img/choco-chip-cookies.jpg'),
        require('../assets/img/strawberry-jam-cookies.jpg'),
        require('../assets/img/blackberry-stuffed-bread.jpg'),
        require('../assets/img/cherry-cake.jpg')
      ],

      counter: 0

    }
  },

  methods: {

    // PREV IMG FUNCTION
    prevImg(){
      this.counter--
      console.log(this.counter);

      if(this.counter < 0){
        this.counter = this.images.length - 1;
      }
      
    },

    // NEXT IMG FUNCTION
    nextImg(){
      this.counter++
      console.log(this.counter);

      if(this.counter > this.images.length - 1){
        this.counter = 0;
      }
    }

  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.product-image-box{
  width: 65%;
  height: 100%;
  display: flex;
  position: relative;

  .item{
    width: 50%;
    padding: 10px;

    img{
      width: 600px;
    }
  }

  // .l-product-image, .r-product-image{
  //   width: 50%;
  //   padding: 10px;

  //   img{
  //     width: 600px;
  //   }
  // }

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
    cursor: pointer;
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

</style>