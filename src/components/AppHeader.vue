<script>
export default {
  data() {
    return {
        headerLinks: [
            {
                section: 'characters',
                url: '#',
                active: false

            },
            {
                section: 'comics',
                url: '#',
                active: true

            },
            {
                section: 'movies',
                url: '#',
                active: false

            },
            {
                section: 'tv',
                url: '#',
                active: false

            },
            {
                section: 'games',
                url: '#',
                active: false

            },
            {
                section: 'collectibles',
                url: '#',
                active: false

            },
            {
                section: 'videos',
                url: '#',
                active: false

            },
            {
                section: 'fans',
                url: '#',
                active: false

            },
            {
                section: 'news',
                url: '#',
                active: false

            },
            {
                section: 'shop',
                url: '#',
                active: false

            },

        ]
    }
  }
}
</script>

<template>
    <nav>
        <div class="header-logo">
            <img src="../img/dc-logo.png" alt="logo dc">
        </div>
        <ul>
            <li v-for="(item, index) in headerLinks" :key="index" :class="(item.active == true) ? 'active' : ''">
                {{ item.section }}
            </li>
           <!--<li>characters</li>
           <li>comics</li>
           <li>movies</li>
           <li>tv</li>
           <li>games</li>
           <li>collectibles</li>
           <li>videos</li>
           <li>fans</li>
           <li>news</li>
           <li>shop</li>-->
        </ul>
    </nav>
</template>

<style lang="scss" scoped>
  @use '../styles/general.scss';
  @use '../styles/partials/mixins' as *;
  @use '../styles/partials/variables' as *;

  nav {
    @include flexHeader;
    

    .header-logo {
        width: 85px;
        
        img {
            width: 100%;
        }
    }
    
    ul {
        display: flex;

        li{
            font-size: 13px;
            text-transform: uppercase;
            padding: 3rem 0;
            margin: 0 1rem;
            color: $grey-font;
            font-weight: bold;

           &.active {
            border-bottom: 5px solid #0076f2;
            color: #0076f2;
           }
        }
    } 
    
  }
    


</style>