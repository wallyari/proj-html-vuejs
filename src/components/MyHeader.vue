<template>
<header class="text-uppercase">

    <div class="nav-bar d-flex align-items-center">
        <!--BTN -->
        <button type="button" class="btn text-white text-uppercase">order online</button>
        <!-- Nav CENTRE -->
        <ul>
        <li>
            <a href="#" class="li-svg ">
                <img class="filter-white" src="../assets/svg/svg-0.svg" alt=""> home
                </a>
            </li>
            <li><a href="#">pages</a></li>
            <li><a href="#">menu</a></li>

            <li>
                <a href="#" id="header-logo" >
                    <img src="../assets/img/h5-logo-divided-header.png" alt="logo-header">
                </a>
            </li>

            <li><a href="#">event</a></li>
            <li><a href="#">blog</a></li>
            <li><a href="#" class="active" >landing</a></li>
        </ul>
            <!-- Nav DX -->
        <ul>
            <li>
                <a href="#" class="li-svg">
                    <span>0</span>
                    <img class="filter-white" src="../assets/svg/svg-1.svg" alt="cart">cart
                </a>
            </li>
            <li>
                <a href="#" class="li-svg">
                    <i class="fas fa-search"></i>search
                </a>
            </li>
        </ul>
    </div>
    
    <!--  Section Jumbotron Header-->
    <div class="jumbotron-header">
        <img src="../assets/img/h3-rev-img-5.png" alt="" class="jumbo-urban">
        <img src="../assets/img/h3-rev-img-6.png" alt="" class="jumbo-urban-tastes">
    </div>   

    </header>
</template>

<script>
export default {
    name:'MyHeader'
}
</script>

<style lang="scss" >

@import "../assets/style/variables.scss";

header{
    height: 500px;
    width: 100vw;
    background-color: $bg-header;
}
//NAVBAR HEADER
#header-logo img{
    width: 100px;
}

.nav-bar {
    height: 100px;
    width: 70%;
    margin: 0 auto;
    justify-content: space-between;
    line-height: 65px;
    margin-bottom: 30px;
}

.nav-bar  ul li{
    list-style: none;
    padding: 0 10px;
    font-size: 12px;
}

.nav-bar  ul li a{
    text-decoration: none;
    color: white;
}

ul li a:hover{
    color: $hover-li-navbar;
}

.nav-bar  ul{
    display: flex;
    padding-top: 20px;
}

.active{
    color: $hover-li-navbar !important;
}

.li-svg img{
    width: 20px;
}

// To change any SVGs color 
.filter-white{
    filter: invert(100%);
    }

.li-svg span{
    bottom: 5px;
    margin-right: -8px;
    background-color: white;
    color: $bg-btn-header;
    border-radius: 70%;
    z-index: 3;
    position: relative;
    padding: 2px 5px;
}


.nav-bar .btn{
    font-size: 10px;
    height: 30px;
    width: 110px;
    border-radius: 0;
    background-color: $bg-btn-header;
}
//JUMBOTRON HEADER
.jumbotron-header{
    width: 45%;
    height: calc(500px - 100px - 30px);
    margin: 0 auto;
    display: flex;
    padding-bottom: 40px;
}

.jumbo-urban-tastes{
    margin-left: -63%;
}


</style>