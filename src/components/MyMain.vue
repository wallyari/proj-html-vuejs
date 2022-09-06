<template>
    <div class="jumbotron">

<!-- jumbo pictures -->
      <div class="jumbotron-main d-flex">
          <img src="../assets/img/h3-img-1.jpg" alt="">
          <img src="../assets/img/h3-img-2.jpg" alt="">
          <img src="../assets/img/h3-img-3.jpg" alt="">
          <img src="../assets/img/h3-img-4.jpg" alt="">
      </div>

<!-- jumbo testimonial -->

      <div class="jumbotron-quote">
          <div class="jumbotron-quote-text text-uppercase">
              <i class="fas fa-quote-left"></i>
              <h4>
                "forget the trendy pizza shops. this hidden spot makes the best new <br> york-style pizza slice in naples"
              </h4>
              <p>
                washington post 2018
              </p>
            </div>

            <div class="jumbotron-quote-logo">
            <img src="../assets/svg/svg-4.svg" alt="pizza cursore">
          </div>
    </div>

    </div>
</template>


<script>
export default {
    name: 'MyMain',
    components: {
       
    }
}
</script>

<style lang="scss" scoped>

@import '../assets/style/variables.scss';

.jumbotron-main{
    width: 100vw;
    background-color: white;
    padding: 3px 0;
}

.jumbotron-main img{
    width: 25%;
    padding: 5px;
}

.jumbotron-quote{
    background-image: url('../assets/img/h3-testimonials-bckgrnd.jpg');
    height: 350px;
    width: 100vw;
    background-position: center;
    background-size: contain;
    justify-content: center;
    align-items: center;
}
.jumbotron-quote-text{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 90%;
}

.jumbotron-quote-logo{
    height: 10%;
    text-align: right;
    margin-top: -20px;
    padding-right: 20px;
}

.jumbotron-quote-logo img{
    background-color: white;
    padding: 11px 15px;
    border-radius: 50%;
    cursor: pointer;
}

.jumbotron-quote-text i{
    color: $color-quote-left;
    font-size: 50px;
}

.jumbotron-quote-text h4,
.jumbotron-quote-text p{
    text-align: center;
    margin-top: 20px;
}

.jumbotron-quote-text p{
    color: $color-quote-newspaper;
    font-size: 12px;
}

</style>