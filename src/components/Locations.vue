<template>
  <section class="locations">
    <h5 class="title-section">LOCATIONS</h5>
    <h2 class="title-2">Visit our Bakeries</h2>

    <div class="store-box">
      <div class="store-image">
        <img src="../assets/img/new-york-bk.jpg" alt="">
      </div>
      <div class="store-text-box new-york">
        <h2 class="title-2">New York</h2>

        <div class="store-info">
          <div class="call-us">
            <p class="title-section">CALL US</p>
            <p class="title-section">1.800.458.556</p>
          </div>
          <div class="open-date">
            <p class="title-section">OPEN ALL WEEK</p>
            <p class="title-section">9.00 AM - 6.00 PM</p>
          </div>
          <div class="store-button">
            <div class="btn btn-white">View Map</div>
          </div>
        </div>
      </div>
    </div>

    <div class="store-box">
      <div class="store-image">
        <img src="../assets/img/london-bk.jpg" alt="">
      </div>
      <div class="store-text-box london">
        <h2 class="title-2">London</h2>

        <div class="store-info">
          <div class="call-us">
            <p class="title-section">CALL US</p>
            <p class="title-section">1.800.458.556</p>
          </div>
          <div class="open-date">
            <p class="title-section">OPEN ALL WEEK</p>
            <p class="title-section">9.00 AM - 6.00 PM</p>
          </div>
          <div class="store-button">
            <div class="btn btn-white">
              <span>View Map</span>
            </div>
          </div>
        </div>
      </div>
    </div>

  </section>
</template>

<script>
export default {
  name: 'Locations'
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.locations{
  margin-bottom: 150px;

  .title-section, .title-2{
    text-align: center;
  }

  .store-box{
    width: 50%;
    display: inline-block;

    .store-text-box{
      padding: 40px 20px 10px 20px;

      .title-2{
        margin-bottom: 30px;
      }

      .store-info{
        display: flex;
        justify-content: space-around;

        .store-button .btn{
          width: 100px;
        }
      }
    }

    .new-york{
      background-color: lighten($blue-color, 73%);
    }

    .london{
      background-color: lighten($beige-color, 18%);
    }

  }
}

</style>