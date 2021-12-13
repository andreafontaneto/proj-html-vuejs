<template>

<div class="jumbotron">
  <Header />

  <div class="container">
    <div class="jumbo-inner">
      <div class="jumbo-text">
        <h5 class="title-section">FRESH & TASTY BAKERY EVERY DAY</h5>
        <h1 class="title-1">The Perfect Fresh Bread</h1>
        <p class="subtitle">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla, obcaecati necessitatibus. Quam aliquid corrupti sed rem. Ratione eius quam temporibus.</p>
        
        <div class="btn btn-white">
          <span>Explore our product</span>
        </div>
      </div>
    </div>
  </div>
</div>
  
</template>

<script>

import Header from './Header.vue';

export default {
  name: 'Jumbotron',
  components: {
    Header
  }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

.jumbotron{
  width: 100vw;
  height: 1000px;
  background-image: url('~@/assets/img/hero-header-bakery.jpg');
  background-size: cover;
  background-position: center;
  margin-bottom: 150px;

  .jumbo-inner{
    height: calc(100vh - 100px);
    display: flex;
    align-items: center;

    .jumbo-text{
      width: 30%;
    }

  }

}

</style>