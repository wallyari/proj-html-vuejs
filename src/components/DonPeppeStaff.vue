<template>
    <div class="Staff">       
    <div class="img-staff">
        <img src="../assets/img/h1-team-1a-700x700.jpg" alt="staff_1">
        <img src="../assets/img/h1-team-2a.jpg" alt="staff_2">
        <img src="../assets/img/h1-team-3a.jpg" alt="staff_3">
        <img src="../assets/img/h1-team-4a.jpg" alt="staff_4">
    </div>
    </div>
</template>

<script>

export default {
    name: 'DonPeppeStaff',
    components:{

    }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/variables.scss';


.img-staff{
    display: flex;
    
    img{
    width: 25%;
    height: auto;
}
}




</style>