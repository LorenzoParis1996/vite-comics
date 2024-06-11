<script>
import AppComics from './AppComics.vue';
export default {
  data() {
    return {}
    },
    components: {
      AppComics
    }
}
</script>

<template>
  <div class="jumbo-main">
  </div>

  
  <div class="content">
    <h1>--> Content goes here <--</h1>
    </div>
  <AppComics/>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss';

.jumbo-main {
   background-image: url(../img/jumbotron.jpg);
   padding: 13rem;
}

.content {
    background-color: #1c1c1c;
    color: white;
    padding: 3rem;
    font-size: 10px;
    
    h1 {
      padding-left: 13rem;
    }
 }
</style>