<template>
    <div class="jumbotron-main">
        <!-- Staff -->
        <ul class="d-flex">
            <li v-for="(staff, index) in imgStaff" :key="index">
            <FourCards :url="staff.url" />
            </li>
        </ul>
    </div>
</template>

<script>
import FourCards from './FourCards.vue';

export default {
    name: "DonPeppeStaff",
    components: {
        FourCards,
    },
    data() {
        return {
        imgStaff: [
            {
            url: require("@/assets/img/h1-team-1a-700x700.jpg"),
            
            },
            {
            url: require("@/assets/img/h1-team-2a.jpg"),
            
            },
            {
            url: require("@/assets/img/h1-team-4a.jpg"),
            
            },
            {
            url: require("@/assets/img/h1-team-3a.jpg"),
            
            },
        ],
        };
    },
    };
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
</style>