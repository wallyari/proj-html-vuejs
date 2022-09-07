<template>
<div class="special d-flex">
    <!-- LOGO & BG SX -->
    <div class="box">
        <div class="img-box">
        <img class="bg-special" src="../assets/img/h1-img-4.jpg" alt="" />
        <img class="logo-special" src="../assets/img/h1-img-7n.png" alt="" />
        </div>
    </div>

    <!-- BOX DX -->
    <div class="combo-list d-flex justify-content-center align-items-center">
        <div class="combo-box">
        <h1 class="title text-uppercase">specials*</h1>
        <div class="special-description">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit.
        </div>
        <div>
            <h3 class="subtitle text-uppercase">
            <span class="price">$10</span> combo piccolo
            </h3>
            <ul>
                <li class="description">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. <br> Aperiam excepturi hic quos!
                </li>
            </ul>
        </div>
        <div>
            <h3 class="subtitle text-uppercase">
                <span class="price">$20</span> combo medium
            </h3>
        <ul>
            <li class="description">
                Lorem ipsum, dolor sit amet consectetur adipisicing elit. <br> Aperiam excepturi hic quos!
                </li>
        </ul>
        </div>
            <div>
                <h3 class="subtitle text-uppercase">
                <span class="price">$30</span> combo grande
                </h3>
                <ul>
                    <li class="description">
                    Lorem ipsum, dolor sit amet consectetur adipisicing elit. <br> Aperiam excepturi hic quos!
                    </li>
                </ul>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
name: "SpecialCombo",
};
</script>

<style lang="scss" scoped>
@import "../assets/style/variables.scss";

.special  {
padding: 8 0;
.box,
  .combo-list{
    width: 50%;
}
.img-box {
    width: 100%;
    height: 100%;
    position: relative;
    img {
    width: 100%;
    }
    .bg-special {
    height: 100%;
    }
    .logo-special {
    width: 40%;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    }
}
.combo-list{
    .combo-box {
    width: 60%;
    .title {
        font-size: 30px;
        font-weight: 500;
    }
    .subtitle {
        font-weight: 400;
        padding-bottom: 3px;
    }
    .price {
        font-weight: 400;
        color: #D2401E;
        padding-right: 10px;
    }
    .special-description {
        padding: 2px 0 30px;
    }
    .special-description,
    .description {
        font-weight: 400;
        width: 76%;
        color: #D2401E;
        letter-spacing: 1px;
    }
    ul {
        list-style-type: none;
        li {
        padding-left: 40px;
        font-size: 15px;
        padding-bottom: 19px;

        }
        }
    }
    }
}
</style>