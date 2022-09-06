<template>
  <div id="app">
    <MyHeader :navLeftLink='navLeftLink' :navRightlink='navRightLink'/>
    <MyMain/>
    <SpecialCombo/>
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import SpecialCombo from './components/SpecialCombo.vue';
import MyFooter from './components/MyFooter.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    MyFooter,
    SpecialCombo,
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
