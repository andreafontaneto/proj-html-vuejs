<template>

  <Jumbotron />
  
</template>

<script>

import Jumbotron from './components/Jumbotron.vue';

export default {
  name: 'App',
  components: {
    Jumbotron
  }
}
</script>

<style lang="scss">

@import url('./assets/style/vars.scss');
@import url('./assets/style/generals.scss');

</style>
