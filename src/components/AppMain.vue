<script>
import AppCard from './AppCard.vue';
export default {
  data() {
    return {}
    },
    components: {
      AppCard
    }
}
</script>

<template>
  <div class="jumbo-main">
  </div>

  
  
  <AppCard/>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss';

.jumbo-main {
   background-image: url(../img/jumbotron.jpg);
   padding: 13rem;
}


</style>