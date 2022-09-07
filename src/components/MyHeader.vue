<template>
<header class="text-uppercase">

    <div class="nav-bar d-flex justify-content-center align-items-center ">
        <!--BTN -->
        <button type="button" class="btn text-white text-uppercase">order online</button>
        <!-- Nav CENTRE -->
        <ul>
        <!-- nav-sinistra     -->
            <li>
                <li v-for="leftLink in navLeftLink" :key="leftLink">

                <a href="#" class="li-svg">
                {{leftLink}}
                </a>

            </li>

            <li>
                <a href="#" id="header-logo" >
                <img src="../assets/img/h5-logo-divided-header.png" alt="logo-navbar">
                </a>
            </li>

            <li v-for="rightLink in navRightLink" :key="rightLink">

                <a href="#" class="li-svg">
                {{rightLink}}
                </a>

            </li>
            <!-- <a href="#" class="li-svg ">
                <img class="filter-white" src="../assets/svg/svg-0.svg" alt=""> home
                </a>
            </li>
            <li><a href="#">pages</a></li>
            <li><a href="#">menu</a></li>

            <li>
                <a href="#" id="header-logo" >
                    <img src="../assets/img/h5-logo-divided-header.png" alt="logo-navbar">
                </a>
            </li>

            <li><a href="#">event</a></li>
            <li><a href="#">blog</a></li>
            <li><a href="#" class="active" >landing</a></li> -->
        </ul>
            <!-- Nav DX -->
        <ul class="cart-search-box">
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
        <div class="img-box d-flex justify-content-center align-items-center">
        <img class="jumbo-urban" src="../assets/img/h3-rev-img-5.png" alt="">
        <img class="jumbo-urban-tastes" src="../assets/img/h3-rev-img-6.png" alt="" >
        </div>
    </div>   

    </header>
</template>

<script>
export default {
    name:'MyHeader',
    data(){
        return{
            navLeftLink:[
                "home",
                "pages",
                "menu",
            ],
            navRightLink:[
                "event",
                "blog",
                "landing",

            ],
        }
        
    }
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
    line-height: 65px;
    margin-bottom: 30px;

    ul{
    display: flex;
    padding-top: 20px;
    }
    
    ul li{
    list-style: none;
    padding: 0 10px;
    font-size: 12px;
    }
    
    a{
    text-decoration: none;
    color: white;
    }
    
    .btn{
    font-size: 10px;
    height: 30px;
    width: 110px;
    border-radius: 0;
    background-color: $bg-btn-header;
    }

}


ul li a:hover{
    color: $hover-li-navbar;
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


//JUMBOTRON HEADER
.jumbotron-header {
    position: relative;
    padding-top: 15px;
    padding-bottom: 15px;
    .img-box {
    padding: 15pxm 0;
    
    .jumbo-urban {
        width: 40%;
        }
    .jumbo-urban-tastes{
        width: 12%;
        position: absolute;
        top: 53%;
        left: 50%;
        transform: translate(-50%, -50%);   

    }    
            
            
        }
}




</style>