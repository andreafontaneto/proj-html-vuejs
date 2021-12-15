<template>
  <footer class="container">

    <div class="footer-left">
      <div :class="logoImage.class">
        <img :src="logoImage.path" :alt="logoImage.name">
      </div>

      <div class="menu-box">
        <ul>
          <li v-for="(link, index) in menuLinks" :key="index"><a :href="menuLinks.url">{{ link.text }}</a></li>
          <!-- <li><a href="#">Shop</a></li>
          <li><a href="#">About</a></li>
          <li><a href="#">Gallery</a></li>
          <li><a href="#">Location</a></li>
          <li><a href="#">Journal</a></li>
          <li><a href="#">Contact</a></li>
          <li><a href="#">Orders</a></li> -->
          <li class="cart">
            <a href="#">
              <i class="fas fa-shopping-cart"></i>
            </a>
            <div class="item-number">
              <span>0</span>
            </div>
          </li>
        </ul>
      </div>

      <p class="subtitle">&copy; {{ credits.copyright }} | {{ credits.theme }} | {{ credits.rights }} | {{ credits.powered }}</p>
    </div>

    <div class="footer-right">
      <h3 class="title-3">Subscribe to our Newsletter</h3>
      <div class="input-box">
        <input type="text" placeholder="Enter email address">
        <div class="btn btn-violet">Subscribe</div>
      </div>
      <div class="social-icons">
        <a href=""><i class="fab fa-instagram"></i></a>
        <a href=""><i class="fab fa-twitter"></i></a>
        <a href=""><i class="fab fa-facebook"></i></a>
        <a href=""><i class="fab fa-pinterest-p"></i></a>
      </div>
    </div>

  </footer>
</template>

<script>
export default {
  name: 'Footer',

  data(){
    return{

      logoImage: {
        name: 'logo',
        class: 'logo-box',
        path: require('../assets/img/avada-bakery-logo-retina.png')
      },

      menuLinks: [

        {
          url: '/shop',
          text: 'Shop'
        },
        {
          url: '/about',
          text: 'About'
        },
        {
          url: '/gallery',
          text: 'Gallery'
        },
        {
          url: '/location',
          text: 'Location'
        },
        {
          url: '/journal',
          text: 'Journal'
        },
        {
          url: '/contact',
          text: 'Contact'
        },
        {
          url: '/orders',
          text: 'Orders'
        }
      ],

      credits: {

        copyright: 'Copyright 2012 - 2020',
        theme: 'Avada Theme by ThemeFusion',
        rights: 'All Rights Reserved',
        powered: 'Powered by Wordpress'

      }

    }
  }

}
</script>

<style lang="scss" scoped>

@import '../assets/style/vars.scss';
@import '../assets/style/generals.scss';

footer{
  display: flex;

  .footer-left, .footer-right{
    width: 50%;

    .logo-box{
      width: 200px;
      margin-left: 20px;
    }

    .menu-box{
      margin-bottom: 100px;

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
            font-size: 14px;
            color: $violet-color;
          }

          .item-number{
            width: 20px;
            height: 20px;
            background-color: $light-violet-color;
            border-radius: 50%;
            text-align: center;
            display: inline-block;

            span{
              color: $violet-color;
              font-size: 12px;
              line-height: 20px;
            }
          }

        }
        
        .cart{
          display: inline-block;
        }
      
      }

    }
  }

  .footer-right{
    display: flex;
    flex-direction: column;
    align-items: flex-end;
    
    .title-3{
      margin-bottom: 50px;
    }

    .input-box{
      display: flex;
      margin-bottom: 190px;

      input{
        width: 400px;
        margin-right: 20px;
        padding: 10px;
        border: 1px solid lightgray;
        border-radius: 5px;
      }

      .btn{
        width: 130px;
      }
    }

    .social-icons a{
      color: $violet-color;
      font-size: 18px;
      margin: 0 20px;
    }
  }

  .subtitle{
    font-size: 12px;
    padding-left: 20px;
  }

}

</style>