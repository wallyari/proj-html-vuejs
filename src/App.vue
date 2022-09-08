<template>
  <div id="app">
    <!-- header -->
    <MyHeader/>
    <!-- MAIN -->
    <main>
    <NewsSection/>
    <QuoteSection/>
    <SpecialCombo/>
    <BuildYourPizza/>
    <DonPeppeStaff/>
    <ClientsLogo/>
    <ChooseFlavor/>
    <PizzaDeals/>
    <BookTable/>
    </main>
    <!-- Footer -->
    <MyFooter/>
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import NewsSection from './components/NewsSection.vue';
import QuoteSection from'./components/QuoteSection.vue';
import SpecialCombo from './components/SpecialCombo.vue';
import BuildYourPizza from './components/BuildYourPizza.vue';
import DonPeppeStaff from './components/DonPeppeStaff.vue';
import ClientsLogo from './components/ClientsLogo.vue';
import ChooseFlavor from './components/ChooseFlavor.vue';
import PizzaDeals from './components/PizzaDeals.vue';
import BookTable from './components/BookTable.vue';
import MyFooter from './components/MyFooter.vue';

export default {
  name: 'App',
  components: {
    MyHeader,
    NewsSection,
    QuoteSection,
    SpecialCombo,
    BuildYourPizza,
    DonPeppeStaff,
    ClientsLogo,
    ChooseFlavor,
    PizzaDeals,
    BookTable,
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
