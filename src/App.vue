<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import MyFooter from './components/MyFooter.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter
  },
  data(){
    return{
     
    }
  },
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
@import '~@fortawesome/fontawesome-free/css/all.css';
@import './assets/style/variables.scss';

</style>
