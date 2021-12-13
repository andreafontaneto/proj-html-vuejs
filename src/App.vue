<template>
  <div>

    <Jumbotron />
    <Main />

  </div>
</template>

<script>

import Jumbotron from './components/Jumbotron.vue';
import Main from './components/Main.vue';

export default {
  name: 'App',
  components: {
    Jumbotron,
    Main
  }
}
</script>

<style lang="scss">

@import './assets/style/vars.scss';
@import './assets/style/generals.scss';

</style>
