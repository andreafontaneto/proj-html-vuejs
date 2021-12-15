<template>
  <section class="social">

    <div class="social-row-1">

      <div class="social-image">
        <img src="../assets/img/social-1.jpg" alt="">
      </div>

      <div class="social-text">
        <h5 class="title-section">MADE FOR SHARING</h5>
        <h2 class="title-2">Let's stay in touch</h2>
        <div class="btn btn-violet">
          <i class="fab fa-instagram"></i>
          <span>Follow Us</span>
        </div>
      </div>

      <div class="social-image">
        <img src="../assets/img/social-2.jpg" alt="">
      </div>

    </div>

    <div class="social-row-2">

      <div class="social-image">
        <img src="../assets/img/social-3.jpg" alt="">
      </div>
      <div class="social-image">
        <img src="../assets/img/social-5.jpg" alt="">
      </div>
      <div class="social-image">
        <img src="../assets/img/social-4.jpg" alt="">
      </div>
      <div class="social-image">
        <img src="../assets/img/social-6.jpg" alt="">
      </div>

    </div>

  </section>
</template>

<script>
export default {
  name: 'Social'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.social{
  margin-bottom: 150px;

  .social-row-1, .social-row-2{
    display: flex;

    .social-image{
      width: calc(25% - 40px);
      margin: 0 20px;
    }

    .social-text{
      width: calc(50% - 30px);
      background-color: lighten($light-violet-color, 18%);
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      margin: 0 15px;

      .title-2{
        margin-bottom: 40px;
      }

      .fa-instagram{
        margin-right: 10px;
      }
    }
  }

  .social-row-1{
    margin-bottom: 40px;
  }

  
}

</style>