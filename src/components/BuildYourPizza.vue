<template>
    <div class="pizza-builder">

    <h3 class="text-uppercase">
        aheas and go <br>
        build yout <br>
        own pizzo <br>
        we wont <br>
        Judge
    </h3>

    <div class="bg-top-left"></div>
    <div class="bg-top-mid"></div>
    <div class="bg-top-right"></div>
    <div class="bg-mid-left"></div>
    <div class="bg-mid-mid"></div>
    <div class="bg-mid-right"></div>
    <div class="bg-low-left"></div>
    <div class="bg-low-mid"></div>
    <div class="bg-low-right"></div>
    </div>
</template>

<script>

export default {
    name: 'PizzaBuilder',
    components:{

    }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/variables.scss';

.pizza-builder{
    width: 100vw;
    margin-top: 4px;
    display: flex;
    flex-wrap: wrap;
    position: relative;
}

h3{
    position: absolute;
    left: 20%;
    top: 15%;
    color: white;
    font-size: 60px;
}

//BG SX
.bg-top-left{
    width: 10%;
    height: 100px;
    background-image: url('../assets/img/h3-background-img.jpg');
    background-position: bottom right;
}
.bg-mid-left{
    width: 10%;
    height: 240px;
    background-image: url('../assets/img/h3-background-img.jpg');
    background-position: top right;
}
.bg-low-left{
    width: 10%;
    height: 100px;
    background-image: url('../assets/img/h3-background-img.jpg');
    background-position: center right;
}

// BG CENTRE
.bg-top-mid{
    width: 84%;
    height: 100px;
    background-image: url('../assets/img/h3-background-img.jpg');
    background-position: bottom center;
}

.bg-mid-mid{
    width: 84%;
    height: 240px;
    background-image: url('../assets/img/h3-background-img.jpg');
    background-position: top center;
    background-size: cover;
}

.bg-low-mid{
    width: 84%;
    height: 100px;
    background-image: url('../assets/img/h3-background-img.jpg');
    background-position: center 70%;
    background-size: cover;
}

// BG RIGHT
.bg-top-right{
    width: 6%;
    height: 100px;
    background-image: url('../assets/img/h3-background-img.jpg');
    background-position: bottom left;
}

.bg-mid-right{
    width: 6%;
    height: 240px;
    background-image: url('../assets/img/h3-background-img.jpg');
    background-position: top left;
}


.bg-low-right{
    width: 6%;
    height: 100px;
    background-image: url('../assets/img/h3-background-img.jpg');
    background-position: center left;
}



</style>