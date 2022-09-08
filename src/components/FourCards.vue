<template>

    <img :src="url" alt="img-card" />

</template>

<script>
export default {
  name: "FourCards",
  props: {
    url: String,
  },
};
</script>






<style lang="scss">

.jumbotron-main {
    padding: 8px 0;
    ul {
    list-style-type: none;

        li {
        position: relative;
        width: calc(100% / 4);
        background-size: contain;
        }
        }
    img{
    width: 100%;
    height: 100%;
    
    }
  }



  
</style>