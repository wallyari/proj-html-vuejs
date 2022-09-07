<template>
<div class="deals-container d-flex text-uppercase">
    <div class="box d-flex justify-content-center align-items-center">
    <!-- LEFT SIDE -->
    <div class="info-box">
        <div class="slogan">made with love</div>
        <h1 class="title">delish pizza deals</h1>
        <div
        class="info d-flex"
        v-for="(event, index) in eventsArray"
        :key="index">
        <div class="date">
            <div class="day">{{ event.day }}</div>
            <div class="month">{{ event.month }}</div>
        </div>
        <div class="event">
            <div class="type">
            {{ event.event }}
            </div>
            <div class="place d-flex align-items-center">
            <i class="fas fa-map-marker-alt"></i> {{ event.place }}
            </div>
        </div>
        </div>
    </div>
    </div>

    <!-- RIGHT SIDE -->
    <div class="comic-bg">
    <img src="../assets/img/h3-img-5a.jpg" alt="" />
    </div>
</div>
</template>

<script>
export default {
name: "PizzaDeals",
data() {
    return {
    eventsArray: [
        {
        day: "02",
        month: "nov",
        event: "traditional neapolitan pies in kyoto pizza mercato",
        place: "204 e. pizzetta tommaso",
        },
        {
        day: "03",
        month: "nov",
        event: "terarazza patio dining space opening this weekend",
        place: "204 e. pizzetta tommaso",
        },
        {
        day: "05",
        month: "nov",
        event: "sienna private dining room with stéphane brunn",
        place: "204 e. pizzetta tommaso",
        },
    ],
    };
},
};
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';


.deals-container {
.box {
    color: $bg-btn-header;
    width: 50%;
    background-color:black ;
    .info-box {
    width: 47%;
    margin-right: 80px;
    .slogan {
        color: $bg-btn-header;
        font-size: 15px;
        letter-spacing: 2px;
    }
    .title {
        color:$background-clients;
        padding-top: 15px;
        font-size: 25px;
        font-weight: 500;
    }
    .info {
        border-bottom: 2px dotted rgb(85, 85, 12);
        padding: 32px 0;
        &:last-child {
        border: none;
        padding-bottom: 0;
        }
        .date {
        padding-right: 32px;
        line-height: 36px;
        text-align: center;
        .day {
            font-size: 35px;
            font-weight: 600;
            color: $bg-btn-header;
        }
        .month {
            font-size: 20px;
            color:white;
        }
        }
        .type {
        font-size: 18px;
        line-height: 28px;
        padding-bottom: 0.7rem;
        color:white;
        }
        .place {
        color: $bg-btn-header;
        font-size: 15px;
        text-transform: capitalize;
        letter-spacing: 2px;
        i {
            font-size: 12px;
            padding-right: 10px;
        }
        }
    }
    }
}
  
.comic-bg {
    width: 50%;
    img {
    width: 100%;
    height: 100%;
    }
}
}
</style>