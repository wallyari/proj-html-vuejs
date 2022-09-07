<template>
  <div id="app">
    <MyHeader/>
    <MyMain/>
    <SpecialCombo/>
    <BuildYourPizza/>
    <DonPeppeStaff/>
    <ChooseFlavor/>
    <PizzaDeals/>
    
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MyMain from './components/MyMain.vue';
import SpecialCombo from './components/SpecialCombo.vue';
import BuildYourPizza from './components/BuildYourPizza.vue';
import DonPeppeStaff from './components/DonPeppeStaff.vue';
import ChooseFlavor from './components/ChooseFlavor.vue';
import PizzaDeals from './components/PizzaDeals.vue';
import MyFooter from './components/MyFooter.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    MyMain,
    SpecialCombo,
    BuildYourPizza,
    DonPeppeStaff,
    ChooseFlavor,
    PizzaDeals,
    MyFooter,
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
