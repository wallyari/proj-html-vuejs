<template>
    <div class="form-container d-flex justify-content-center align-items-center">
        <div class="box text-uppercase d-flex align-items-center">
        <div>
            <input type="text" placeholder="1 Person" />
            <i class="fas fa-user-friends"></i>
        </div>
        <span>for</span>
        <div>
            <input type="text" placeholder="11/29/2020" />
            <i class="far fa-calendar"></i>
        </div>
        <span>at</span>
        <div>
            <input type="text" placeholder="7:00 pm" />
            <i class="far fa-clock"></i>
        </div>
        <span></span>
        <button class="btn text-uppercase">book a table</button>
        <div class="sponsor">*Powered by OpenTable</div>
        </div>
    </div>
</template>

<script>
    export default {
    name: "BookTable",
    };
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';


.form-container {
    margin: 8px 0;
    background-image: url(../assets/img/h3-background-img-3.jpg);
    color: white;
    background-size: cover;
.box {
    padding: 80px;
    position: relative;
    span {
        width: 50px;
        text-align: center;
        font-size: 15px;
    }
    input {
        padding: 15px 80px 12px 15px;
        border: 2px solid black;        
        font-size: 13px;
        color: grey;
    }
    div {
        position: relative;
        i {
        position: absolute;
        right: 7%;
        top: 38%;
        color: white;
        font-size: 13px;
        }
        }
    .sponsor {
        font-size: 10px;
        font-weight: 300;
        position: absolute;
        bottom: 26%;
        }
    .btn {
        padding: 20px 60px;
        font-size: 10px;
    }
    }
}
</style>