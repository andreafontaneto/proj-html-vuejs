<template>
  <section class="bakery-process">
    <div class="bp-image-01">

      <div class="bp-inner-left">
        <h1 class="title-1">Tell us what you have in mind</h1>
      </div>

      <div class="bp-inner-right">
        <div class="bp-number">
          <span class="number">01</span>
        </div>
        <div class="bp-description">
          <h5 class="title-section">MANUAL INGREDIENTS SELECTION</h5>
          <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto iure, sunt nulla asperiores non ipsam, tempora illo hic dolores soluta earum possimus eius quibusdam, amet minima culpa sint at quae. Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto iure, sunt nulla asperiores non ipsam.</p>
        </div>
      </div>

    </div>

    <div class="bp-center">

      <div class="bp-image-02">

        <div class="bp-inner-center">
          <div class="title-box">
            <h1 class="title-1">We Start Baking</h1> 
            <span class="number">02</span>
          </div>
          <div class="bp-description">
            <h5 class="title-section">SWEET & DELICIOUS</h5>
            <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit a incidunt quod. Molestiae vitae consequuntur ratione ea porro aut doloremque voluptatem, fugit saepe soluta accusantium ut, sint tempore eum perspiciatis.</p>
          </div>
        </div>

      </div>

      <div class="bp-text">
        <h5 class="title-section">DON'T JUST TAKE OUR WORD FOR IT</h5>
        <h1 class="title-1">
          "Finally found an alternative to the mass produced products. Something that incorporates real organic ingredients, nutriend dense wellness while promoting sustainability and activity"
        </h1>
        <span class="title-section">Rachel Cooper, Founder</span>
      </div>

    </div>

    <div class="bp-image-03">

      <div class="bp-inner-left">
        <h1 class="title-1">Delivered to your home</h1>

        <div class="bp-description">
          <h5 class="title-section">BAKED TO ORDER & GIFT WRAPPED</h5>
          <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto iure, sunt nulla asperiores non ipsam, tempora illo hic dolores soluta earum possimus eius quibusdam, amet minima culpa sint at quae. Lorem ipsum dolor sit amet consectetur adipisicing elit. Iusto iure, sunt nulla asperiores non ipsam.</p>
        </div>
      </div>

      <div class="bp-inner-right">
        <div class="bp-number">
          <span class="number">03</span>
        </div>
      </div>

    </div>
  </section>
</template>

<script>
export default {
  name: 'BakeryProcess'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.bakery-process{
  margin-bottom: 150px;

  .title-1{
    color: white;
  }

  .number, .subtitle{
    color: white;
  }

  .bp-number{
    display: flex;
    justify-content: flex-end;
  }

  .number{
    font-size: 100px;
  }

  .title-section{
    color: lighten($grey-color, 10%);
  }

  .bp-image-01, .bp-image-03{
    width: 100%;
    height: 800px;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    display: flex;

    .bp-inner-left, .bp-inner-right{
      width: 50%;
      padding: 100px;
      display: flex;
      justify-content: space-between;
      flex-direction: column;
      background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.6)); 
    }

  }

  .bp-image-01{
    background-image: url('~@/assets/img/bakery-process-1.jpg');
  }

  .bp-image-03{
    background-position: center;
    background-image: url('~@/assets/img/bakery-process-3.jpg');
  }

  .bp-center{
    width: 100%;
    height: 800px;
    margin: 40px 0;
    display: flex;

    .bp-image-02{
      width: 50%;
      height: 100%;
      background-image: url('~@/assets/img/bakery-process-2.jpg');
      background-position: center;
      background-size: cover;
      display: flex;
      flex-direction: column;
      justify-content: space-between;

      .bp-inner-center{
        width: 100%;
        height: 100%;
        padding: 70px;
        background-image: linear-gradient(to bottom, rgba(0, 0, 0, 0.3), rgba(0, 0, 0, 0.6));

        .title-box{
          display: flex;
          justify-content: space-between;
          align-items: flex-start;
        }

        .bp-description{
          width: 50%;

          .title-section{
            color: lighten($grey-color, 30%);
          }
        }
      }

    }
  
    .bp-text{
      width: 50%;
      height: 100%;
      background-color: lighten($light-violet-color, 18%);
      margin-left: 30px;
      padding: 80px;
      display: flex;
      flex-direction: column;
      justify-content: center;

      .title-section, .title-1{
        margin-bottom: 40px;
      }

      .title-1{
        color: $violet-color;
      }
    }
  }

}

</style>