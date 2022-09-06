<template>
    <div class="specials d-flex">
        <div class="specials-combo-img">
            <img src="../assets/img/h1-img-7n.png" alt="">
        </div>
        <div class="specials-pizza">


        </div>
    </div>
</template>

<script>
export default {
    name: 'SpecialCombo',
    components: {

    }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/variables.scss';

.specials{
    height: 600px;
    width: 90vw;
    background-color: white;
    padding: 10px;
}

.specials-combo-img{
    background-image: url('../assets/img/h1-img-4.jpg');
    background-size: cover;
    width: 50%;
    display: flex;
    justify-content: center;
    align-items: center;
}


</style>