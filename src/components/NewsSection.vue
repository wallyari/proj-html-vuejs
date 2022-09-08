<template>

<!-- JUMBO IMG -->
    <div class="jumbotron-main">
        <ul class="d-flex">
            <li
            v-for="(card,index) in imgCards" 
            :key="index">
            <FourCards :url="card.url" />
            </li>
        </ul>
    </div>

<!-- JUMBO QUOTE -->

</template>


<script>
import FourCards from "@/components/FourCards.vue";

export default {
  name: "NewsSection",
  components: {
    FourCards,
  },
  data() {
    return {
    imgCards: [
        {
            url: require("@/assets/img/h3-img-1.jpg"),
        },
        {
            url: require("@/assets/img/h3-img-2.jpg"),
        },
        {
            url: require("@/assets/img/h3-img-3.jpg"),
        },
        {
            url: require("@/assets/img/h3-img-4.jpg"),
        },
    ],
    };
},
};
</script>

<style lang="scss" scoped>

@import '../assets/style/variables.scss';

// .jumbotron-main {
//     padding: 8px 0;
//     ul {
//     list-style: none;
//         li {
//         position: relative;
//         width: calc(98.5% / 4);
//         background-size: contain;
//         }
//         }
//     }

// img{
//     width: 100%;
//     height: 100%;
    
    

// }


</style>