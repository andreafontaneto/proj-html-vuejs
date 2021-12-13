<template>

<div class="jumbotron">
  <Header />
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

//@import url('./assets/style/vars.scss');
@import url('../assets/style/generals.scss');

.jumbotron{
  width: 100vw;
  height: 1000px;
  background-image: url('~@/assets/img/hero-header-bakery.jpg');
  background-size: cover;
  background-position: center;
}

</style>