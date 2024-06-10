<script>
export default {
  data() {
    return {
      dcComicsLinks: [
        {
          section:'characters',
          url: '#',
          active: false
        },
        {
          section:'comics',
          url: '#',
          active: false
        },
        {
          section:'movies',
          url: '#',
          active: false
        },
        {
          section:'tv',
          url: '#',
          active: false
        },
        {
          section:'games',
          url: '#',
          active: false
        },
        {
          section:'videos',
          url: '#',
          active: false
        },
        {
          section:'news',
          url: '#',
          active: false
        }
      ],
      shopLinks: [
        {
          section:'shop dc',
          url: '#',
          active: false
        },
        {
          section:'shop dc collectibles',
          url: '#',
          active: false
        }
      ],
      dcLinks: [
          {
          section:'terms of use',
          url: '#',
          active: false
        },
        {
          section:'privacy policy (new)',
          url: '#',
          active: false
        },
        {
          section:'ad choices',
          url: '#',
          active: false
        },
        {
          section:'advertising',
          url: '#',
          active: false
        },
        {
          section:'jobs',
          url: '#',
          active: false
        },
        {
          section:'subscriptions',
          url: '#',
          active: false
        },
        {
          section:'talent workshops',
          url: '#',
          active: false
        },
        {
          section:'cpsc certificates',
          url: '#',
          active: false
        },
        {
          section:'rating',
          url: '#',
          active: false
        },
        {
          section:'shop help',
          url: '#',
          active: false
        },
        {
          section:'contact us',
          url: '#',
          active: false
        }
      ],
      sitesLinks: [
        {
          section:'dc',
          url: '#',
          active: false
        },
        {
          section:'mad magazine',
          url: '#',
          active: false
        },
        {
          section:'dc kids',
          url: '#',
          active: false
        },
        {
          section:'dc universe',
          url: '#',
          active: false
        },
        {
          section:'dc power visa',
          url: '#',
          active: false
        }
      ]
    }
   }
}
</script>

<template>
 <div class="container">
  <div class="lists">
  <nav>
    <p>dc comics</p>
    <ul class="margin-bottom">
      <li v-for="(item, index) in dcComicsLinks" :key="index">
        {{ item.section }}
      </li>
      <!--<li>characters</li>
      <li>comics</li>
      <li>movies</li>
      <li>tv</li>
      <li>games</li>
      <li>videos</li>
      <li>news</li>-->
    </ul>

    <p>shop</p>
    <ul>
      <li v-for="(item, index) in shopLinks" :key="index">
        {{ item.section }}
      </li>
      <!--<li>shop dc</li>
      <li>shop dc collectibles</li>-->
    </ul>
  </nav>

  <nav>
    <p>dc</p>
    <ul>
      <li v-for="(item, index) in dcLinks" :key="index">
        {{ item.section }}
      </li>
      <!--<li>terms of use</li>
      <li>privacy policy (new)</li>
      <li>ad choices</li>
      <li>advertising</li>
      <li>jobs</li>
      <li>subscriptions</li>
      <li>talent workshops</li>
      <li>cpsc certificates</li>
      <li>rating</li>
      <li>shop help</li>
      <li>contact us</li>-->
    </ul>
  </nav>

  <nav>
    <p>sites</p>
    <ul>
      <li v-for="(item, index) in sitesLinks" :key="index">
        {{ item.section }}
      </li>
     <!--<li>dc</li>
     <li>mad magazine</li>
     <li>dc kids</li>
     <li>dc universe</li>
     <li>dc power visa</li>-->
    </ul>
  </nav>
  </div>

  <div class="img-container">
    <img src="../img/dc-logo-bg.png" alt="dc logo">
  </div>
 </div>

 <section>
  <nav>
    <div>
      <button>sign-up now!</button>
    </div>
    <div class="socials">
      
      <ul>
          <p>follow us</p>        
          <li><img src="../img/footer-facebook.png" alt=""></li>
          <li><img src="../img/footer-twitter.png" alt=""></li>
          <li><img src="../img/footer-youtube.png" alt=""></li>
          <li><img src="../img/footer-pinterest.png" alt=""></li>
          <li><img src="../img/footer-periscope.png" alt=""></li>
      </ul>
    </div>
  </nav>
 </section>
</template>

<style lang="scss" scoped>
  @use '../styles/general.scss';
  @use '../styles/partials/variables' as *;
  @use '../styles/partials/mixins' as *;
  

  .container {
    padding: 1.5rem;
    display: flex;
    justify-content: space-around;
    align-items: center;
    background-image: url(../img/footer-bg.jpg);
    background-repeat: no-repeat;
    background-size: cover;
  }

  .lists {
    display: flex;
     nav {
      margin: 0 1rem;
      ul>li {
        color: $grey-font;
        font-size: 15px;
        text-transform: capitalize;
      }
      .margin-bottom {
        margin-bottom: 0.8rem;
      }
     }

     p {
      margin-bottom: 0.8rem;
      color: white;
      text-transform: uppercase;
      font-weight: bold;
     }
  }

  .img-container {
    width: 500px;
    img {
      width: 100%;
    }  
  }


  section {
    padding: 2rem;
    background-color: #303030;
    nav {
      @include flexFooter;

      ul {
        display: flex;
        align-items: center;
      } li {
        padding: 0 0.5rem;
      }

      p {
        font-size: 25px;
        text-transform: uppercase;
        color: #067ae5;
        padding: 0 2rem;
      }
    }

    button{
      padding: 0.5rem;
      font-size: 30px;
      border: 3px solid #067ae5;
      color: white;
      text-transform: uppercase;
      background-color: #303030;

      &:hover {
        background-color: gray;
      }
    }

  }

</style>