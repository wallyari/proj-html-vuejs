<template>
    <div class="choose-box">
        <div class="d-flex justify-content-center align-items-centert">
        <!-- TITLE -->
        <div class="title">
            <div class="subtitle text-uppercase">choose your flavour</div>
            <h1 class="text-uppercase">the best pizza menu in town</h1>
            <p class="description">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Fuga dolorum nihil ab illo veritatis officia ut a nemo recusandae! Dolores?
            </p>
        </div>
        </div>

        <!-- PIZZE -->
        <ul class="d-flex">
                <li class="text-uppercase" v-for="(pizza, indice) in pizzasArray" :key="indice">
                <img :src="pizza.url" alt="" />
                <h4>{{ pizza.name }}</h4>
                <span v-show="pizza.strikePrice" class="strike-price"> $65.00 </span>
                <span class="price1">{{ pizza.price }}</span>
                <div v-show="pizza.sold" class="sold-out">
                <span>sold</span>
                </div>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    name: "ChooseFlavor",
    data() {
        return {
        pizzasArray: [
            {
            url: require("../assets/img/h3-product-img-1a-100x100.png"),
            name: "bismark",
            price: "$55.00",
            strikePrice: true,
            sold: false,
            },
            {
            url: require("../assets/img/h3-product-img-2a-150x150.png"),
            name: "fiori di zucca",
            price: "$7.00 - $55.00",
            sold: false,
            },
            {
            url: require("../assets/img/h3-product-img-3a-150x150.png"),
            name: "valdostana",
            price: "$55.00",
            sold: true,
            },
            {
            url: require("../assets/img/h3-product-img-4a-150x150.png"),
            name: "pizza tartufato",
            price: "$45.00",
            sold: false,
            },
            {
            url: require("../assets/img/h3-product-img-5a-150x150.png"),
            name: "francescana",
            price: "$25.00",
            sold: false,
            },
            {
            url: require("../assets/img/h3-product-img-6a-100x100.png"),
            name: "campagnola",
            price: "$55.00 - $95.00",
            sold: false,
            },
            {
            url: require("../assets/img/h3-product-img-5a-150x150.png"),
            name: "lello",
            price: "$55.00",
            sold: false,
            },
            {
            url: require("../assets/img/h3-product-img-6a-100x100.png"),
            name: "deliziosa",
            price: "$55.00",
            sold: true,
            },
        ],
        };
    },
    };
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

    .choose-box {
    padding-bottom: 80px;
    .title {
        text-align: center;
        width: 24%;
        padding: 70px 0 30px;
        
        
        .subtitle {
        font-weight: 600;
        font-size: 15px;
        letter-spacing: 2px;
        word-spacing: 2px;
        color:$bg-btn-header;
        }
        h1 {
        font-weight: 500;
        font-size: 30px;
        padding: 10px 0 15px;
        }
        .description {
        color: black;
        font-weight: 300;
        }
    }
    ul {
        overflow: scroll;
        letter-spacing: 2px;
        line-height: 21px;
        position: relative;
        list-style-type: none;
        h4 {
        color: rgb(45, 43, 43);
        font-weight: 400;
        font-size: 15px;
        padding-top: 12px;
        font-weight: 600;
        }
        .price1 {
        color: rgb(186, 131, 28);
        font-size: 14px;
        font-weight: 600;

        }
        .strike-price {
        text-decoration: line-through;
        font-size: 14px;
        color: grey;
        padding-right: 0.10px;
        font-weight: 600;
        }
        li {
        text-align: center;
        padding: 45px;
        position: relative;
        }
        img {
            width: 200px;
            cursor: pointer;
        }
        }
        .sold-out {

        span {
            background-color: $bg-btn-header;
            border-radius: 70%;
            color: white;
            font-size: 10px;
            top: 10%;
            right: 22.5%;
            padding: 15px 7px; ;
        }
        span {
            position: absolute;
        }
        }
    }
    
</style>