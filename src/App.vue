<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  data() {

  },
  components: {
    AppHeader,
    AppMain,
    AppFooter,
  }
}
</script>

<template>
  <header>
   <AppHeader/>
  </header>
  
  <main>
   <AppMain/>
  </main>

  <footer>
   <AppFooter/>
  
  </footer>
</template>

<style lang="scss">
@use './styles/general.scss'

</style>
