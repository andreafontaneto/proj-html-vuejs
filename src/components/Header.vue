<template>
  <header>
    <div :class="logoImage.class">
      <a href=""><img :src="logoImage.path" :alt="logoImage.name"></a>
    </div>

    <div class="menu-box">
      <ul>
        <li v-for="(link, index) in menuLinks" :key="index">
          <a :class="{active : link.current === true}" :href="link.url">{{ link.text }}</a>
        </li>
        <!-- <li><a class="active" href="#">Home</a></li>
        <li><a href="#">Shop</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Gallery</a></li>
        <li><a href="#">Location</a></li>
        <li><a href="#">Journal</a></li>
        <li><a href="#">Contact</a></li>
        <li><a href="#">My Account</a></li> -->
        <li>
          <a href="#">
            <i class="fas fa-shopping-cart"></i>
          </a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'Header',
  data(){
    return{

      logoImage: {
        name: 'logo',
        class: 'logo-box',
        path: require('../assets/img/avada-bakery-logo-retina.png')
      },

      menuLinks: [

        {
          url: '/home',
          text: 'Home',
          current: false
        },
        {
          url: '/shop',
          text: 'Shop',
          current: true
        },
        {
          url: '/about',
          text: 'About',
          current: false
        },
        {
          url: '/gallery',
          text: 'Gallery',
          current: false
        },
        {
          url: '/location',
          text: 'Location',
          current: false
        },
        {
          url: '/journal',
          text: 'Journal',
          current: false
        },
        {
          url: '/contact',
          text: 'Contact',
          current: false
        },
        {
          url: '/my-account',
          text: 'My Account',
          current: false
        }

      ]
    }
  }
}
</script>

<style lang="scss" scoped>

@import '~@fortawesome/fontawesome-free/css/all.min.css';

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

header{
  width: 100vw;
  margin: 0 20px;
  padding-top: 15px;
  display: flex;
  justify-content: space-between;
  align-content: center;

  .logo-box{
    width: 200px;
    margin-left: 20px;
  }

  .menu-box{
    margin-right: 20px;

    ul{
      margin: 0;
      list-style: none;
      display: flex;

      li{
        margin: 0 5px;
        padding: 0px 15px;

        a{
          padding: 5px;
          text-decoration: none;
          line-height: 100px;
          text-transform: uppercase;
          font-size: 12px;
          font-weight: 600;
          color: $violet-color;
        }

        .active{
          border-bottom: 2px solid $violet-color;
        }

      } 
    
    }

  }
  
}

</style>