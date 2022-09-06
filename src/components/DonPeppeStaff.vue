<template>
    <div class="Staff pt-2">       
    <div class="img-staff">
        <img src="../assets/img/h1-team-1a-700x700.jpg" alt="staff_1">
        <img src="../assets/img/h1-team-2a.jpg" alt="staff_2">
        <img src="../assets/img/h1-team-3a.jpg" alt="staff_3">
        <img src="../assets/img/h1-team-4a.jpg" alt="staff_4">
    </div>
    <!-- Logo Clients -->
    <div class="clients pt-2">
        <div class="logo-clients">
            <img src="../assets/img/h1-clients-img-4.png" alt="clients_1">
            <img src="../assets/img/h1-clients-img-3.png" alt="clients_2">
            <img src="../assets/img/h1-clients-img-1.png" alt="clients_3">
            <img src="../assets/img/h1-clients-img-2.png" alt="clients_4">
            <img src="../assets/img/h1-clients-img-5.png" alt="clients_5">
        </div>
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

//Don Peppe Staff
.img-staff{
    display: flex;
    
    img{
    width: 25%;
    height: auto;
}
}

//Clients Logo
.clients{
    width: 100vw;
    height: 200px;
    background-color: $background-clients;
    display: flex;
    justify-content: center;
    align-items: center;
}
.logo-clients img{
    width: calc(100% / 5);
}

</style>