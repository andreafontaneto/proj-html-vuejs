<template>
  <section class="call-to-action">
    <h5 class="title-section">TRY OUR SEASONAL PRODUCTS</h5>
    <h1 class="title-1">Order for pick-up or delivery to<br>your home</h1>
    <div class="btn btn-white">
      <span>Shop Now</span>
    </div>
  </section>
</template>

<script>
export default {
  name: 'CallToAction'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.call-to-action{
  width: 100vw;
  height: 500px;
  background-image: url('../assets/img/call-to-action-bg.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  padding: 100px 100px 100px 350px;
  margin-bottom: 50px;

  .title-section{
    color: lighten($grey-color, 30%);
  }

  .title-1{
    color: white;
    margin-bottom: 80px;
  }

  .btn{
    padding: 20px;

    span{
      font-size: 18px;
    }
  }
}

</style>