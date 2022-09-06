<template>
    <!-- Bg IMG + logo -->
    <div class="specials d-flex">
        <div class="specials-combo-img">
            <img src="../assets/img/h1-img-7n.png" alt="">
        </div>
        <div class="specials-pizza">

    <!-- Specials Combo Menu-->
    <div class="specials-pizza text-uppercase">

        <div class="specials-pizza-title">
            <h3>specials*</h3>
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
        </div>

        <div class="pizza pizza-combo-p">
            <h4 class="price">
                $10
            </h4>
            <h4 class="name">
                combo piccolo
            </h4>
        </div>
        <span>Lorem ipsum, dolor sit amet consectetur adipisicing elit. <br> Aperiam excepturi hic quos!</span>

        <div class=" pizza pizza-combo-m">
            <h4 class="price">
                $20
            </h4>
            <h4 class="name">
                combo medium
            </h4>
        </div>
        <span>Lorem ipsum, dolor sit amet consectetur adipisicing elit. <br> Aperiam excepturi hic quos!</span>

        <div class="pizza pizza-combo-g">
            <h4 class="price">
                $30
            </h4>
            <h4 class="name">
                combo grande
            </h4>
        </div>
        <span>Lorem ipsum, dolor sit amet consectetur adipisicing elit. <br> Aperiam excepturi hic quos!</span>
    </div>




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

//Special Combo text section
.specials-pizza{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    width: 40%;
    margin: 0 auto;
    position: relative;
}

.specials-pizza span{
    color: rgb(118, 114, 114);
    font-size: 10px;
    text-transform: lowercase;
    margin-left: 130px;
}

.specials-pizza-title p{
    color: rgb(118, 114, 114);
    font-size: 10px;
    text-transform: lowercase;
}

.specials-pizza-title{
    text-align: left;
    margin-left: 10px;
}

.pizza{
    display: flex;
    margin-top: 10px;
}



.pizza .price{
    color: $color-quote-newspaper;
    margin-right: 15px;
}

.jumbo-menu-logo img{
    background-color: white;
    padding: 11px 15px;
    border-radius: 50%;
    cursor: pointer;
    transform: translateY(800%);   
    margin-right: 20px;
}



</style>