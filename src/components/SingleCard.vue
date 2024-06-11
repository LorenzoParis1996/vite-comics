<script>
export default {
    data() {
        return {

        }
    },
    props: {
        singleCard: {
            type: Object,
            required: true
        }
    }
}

</script>

<template>

    <article>
        <img :src="singleCard.thumb" :alt="singleCard.series">
        <p>{{ singleCard.series }}</p>
    </article>

</template>

<style lang="scss" scoped>

article {
        width: calc(100%/ 6);
        padding: 0.8rem;

        img {
          width: 100%;
          height: 200px;
          object-fit: cover;
          object-position: top;

          &:hover {
            filter: brightness(1.50);
          }
          
        }

        p {
          padding-top: 0.5rem;
          color: white;
          text-transform: uppercase;
          font-size: 12px;
        }
      }

</style>