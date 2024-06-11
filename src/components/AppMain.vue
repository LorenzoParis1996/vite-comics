<script>
import AppCards from './AppCards.vue';
export default {
  data() {
    return {}
    },
    components: {
      AppCards
    }
}
</script>

<template>
  <div class="jumbo-main">
  </div>
  <AppCards/>
</template>

<style lang="scss" scoped>
@use '../styles/general.scss';

.jumbo-main {
   background-image: url(../img/jumbotron.jpg);
   height: 26rem;
}


</style>