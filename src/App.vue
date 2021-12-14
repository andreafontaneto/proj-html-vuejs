<template>
  <div>

    <Jumbotron />
    <Main />
    <Footer />

  </div>
</template>

<script>

import Jumbotron from './components/Jumbotron.vue';
import Main from './components/Main.vue';
import Footer from './components/Footer.vue';

export default {
  name: 'App',
  components: {
    Jumbotron,
    Main,
    Footer
  }
}
</script>

<style lang="scss">

@import './assets/style/vars.scss';
@import './assets/style/generals.scss';

</style>
