<script>
export default {
  data() {
    return {}
   }
}
</script>

<template>
 <div class="container">
  <div class="lists">
  <nav>
    <p>dc comics</p>
    <ul>
      <li>characters</li>
      <li>comics</li>
      <li>movies</li>
      <li>tv</li>
      <li>games</li>
      <li>videos</li>
      <li>news</li>
    </ul>

    <p>shop</p>
    <ul>
      <li>shop dc</li>
      <li>shop dc collectibles</li>
    </ul>
  </nav>

  <nav>
    <p>dc</p>
    <ul>
      <li>terms of use</li>
      <li>privacy policy (new)</li>
      <li>ad choices</li>
      <li>advertising</li>
      <li>jobs</li>
      <li>subscriptions</li>
      <li>talent workshops</li>
      <li>cpsc certificates</li>
      <li>rating</li>
      <li>shop help</li>
      <li>contact us</li>
    </ul>
  </nav>

  <nav>
    <p>sites</p>
    <ul>
     <li>dc</li>
     <li>mad magazine</li>
     <li>dc kids</li>
     <li>dc universe</li>
     <li>dc power visa</li>
    </ul>
  </nav>
  </div>

  <div class="img-container">
    <img src="../img/dc-logo-bg.png" alt="dc logo">
  </div>
 </div>
</template>

<style lang="scss" scoped>
  @use '../styles/general.scss';
  

  .container {
    padding: 1.5rem;
    display: flex;
    justify-content: space-around;
    align-items: center;
  }

  .lists {
    display: flex;
     nav {
      margin: 0 1rem;
     }
  }

  .img-container {
    width: 500px;
    img {
      width: 100%;
    }
  }

</style>