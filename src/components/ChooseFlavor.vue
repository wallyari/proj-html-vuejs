<template>
    <div class="choose-flavor">
        <!-- intro choose pizza -->
        <div class="header-flavor">
            <h6>choose your flavour</h6>
            <h2>the best pizza menu in town</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga dolorum nihil <br> ab illo veritatis officia ut a nemo recusandae! Dolores?</p>
        </div>

        <div class="jumbotron-title-logo">
            <img src="../assets/svg/svg-4.svg" alt="">
        </div>

        <!-- lista pizze -->
        <div class="list-pizza">
            <!-- single pizza div -->
            <div class="card-pizza">
                <img src="../assets/img/h3-product-img-1a-100x100.png" alt="">
                <h3>bismark</h3>
                <div class="price">
                <span class="first-price strike">$5.00</span><span class="second-price">$30.00</span>
                </div>
            </div>

            <div class="card-pizza">
                <img src="../assets/img/h3-product-img-2a-150x150.png" alt="">
                <h3>fiori di zucca</h3>
                <div class="price">
                <span class="first-price">$7.00</span><span class="second-price">$50.00</span>
                </div>
            </div>

            <div class="card-pizza">
                <div class="sold">
                sold
                </div>
                <img src="../assets/img/h3-product-img-6a-100x100.png" alt="">
                <h3>valdostana</h3>
                <div class="price">
                <span class="second-price">$55.00</span>
                </div>
            </div>

            <div class="card-pizza">
                <img src="../assets/img/h3-product-img-4a-150x150.png" alt="">
                <h3>pizza tartufat</h3>
                <div class="price">
                <span class="second-price">$45.00</span>
            </div>
            </div>

            <div class="card-pizza">
                <img src="../assets/img/h3-product-img-5a-150x150.png" alt="">
                <h3>francescana</h3>
                <div class="price">
                <span class="second-price">$25.00</span>
            </div>
            </div>

        <div class="card-pizza">
                <img src="../assets/img/h3-product-img-3a-150x150.png" alt="">
                <h3>campagnola</h3>
                <div class="price">
                <span class="first-price">$50.00</span><span class="second-price">$95.00</span>
            </div>
        </div>

        <div class="card-pizza">
            <img src="../assets/img/h3-product-img-1a-100x100.png" alt="">
            <h3>diavola</h3>
            <div class="price">
                <span class="first-price strike">$5.00</span><span class="second-price">$30.00</span>
            </div>
        </div>

        <div class="card-pizza">
            <img src="../assets/img/h3-product-img-2a-150x150.png" alt="">
            <h3>quattro formaggi</h3>
            <div class="price">
                <span class="first-price">$7.00</span><span class="second-price">$50.00</span>
        </div>
        </div>

        <div class="card-pizza">
            <div class="sold">
                sold
            </div>
            <img src="../assets/img/h3-product-img-6a-100x100.png" alt="">
            <h3>funghi</h3>
            <div class="price">
                <span class="second-price">$55.00</span>
            </div>
        </div>

        <div class="card-pizza">
            <img src="../assets/img/h3-product-img-4a-150x150.png" alt="">
            <h3>verdure</h3>
            <div class="price">
                <span class="second-price">$45.00</span>
            </div>
        </div>

        <div class="card-pizza">
            <img src="../assets/img/h3-product-img-5a-150x150.png" alt="">
            <h3>pescatora</h3>
            <div class="price">
                <span class="second-price">$25.00</span>
            </div>
        </div>

        <div class="card-pizza">
            <div class="sold">
                sold
            </div>
            <img src="../assets/img/h3-product-img-3a-150x150.png" alt="">
            <h3>patatine</h3>
            <div class="price">
                <span class="first-price">$50.00</span><span class="second-price">$95.00</span>
            </div>
        </div>

    </div>
    </div>
</template>

<script>

export default {
    name: 'choose-flavor',
    components:{

    }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/variables.scss';

.choose-flavor{
    height: 500px;
}

.header-flavor{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    h6{
    padding-top: 50px;
    text-transform: uppercase;
    color: $color-quote-newspaper;
    font-size: 10px;
    }
    h2{
    text-transform: uppercase;
    }
    p{
    text-align: center;
    color: grey;
    font-size: 12px;
    }   
}


.jumbotron-title-logo{
    height: 10%;
    text-align: right;
    margin-top: -20px;
    padding-right: 20px;
    
    img{
    background-color: white;
    padding: 11px 15px;
    border-radius: 50%;
    cursor: pointer;
    }
    img:hover{
    background-color: lightgray
    }
}

.list-pizza{
    width: 100vw;
    display: flex;
    overflow-x: scroll;
    margin-bottom: 70px;
    padding-bottom: 20px;
}

.card-pizza{
    height: auto;
    min-width: 16%;
    display: flex;
    flex-direction: column;
    text-align: center;
    margin-right: 30px;
    position: relative;
    img{
    width: 100%;
    }
    h3{
    padding-top: 15px;
    color:$color-quote-left;
    text-transform: uppercase;
    font-size: 18px;
    }
}

.sold{
    position: absolute;
    color: white;
    background-color: $bg-btn-header;
    border-radius: 50%;
    padding: 15px 7px;
    text-transform: uppercase;
    right: 25px;
}


.first-price{
    color: $color-quote-newspaper;
    padding-right: 10px;
}

.second-price{
color: $color-quote-newspaper; 
}

.strike.first-price{
    text-decoration:line-through;
    color: grey;
}

</style>