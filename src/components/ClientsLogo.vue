<template>
    <!-- Logo Clients -->
    <div class="container-logo">
        <ul class="clients-box d-flex justify-content-center">
            <li v-for="(client, index) in clientsArray" :key="index">        
            <img :src="client.url" alt="" />
            </li>
        </ul>
    </div>
 
</template>

<script>
export default {
    name: "ClientsLogo",
    data() {
        return {
        clientsArray: [
            {
            url: require("@/assets/img/h1-clients-img-4.png"),
            },
            {
            url: require("@/assets/img/h1-clients-img-3.png"),
            },
            {
            url: require("@/assets/img/h1-clients-img-1.png"),
            },
            {
            url: require("@/assets/img/h1-clients-img-2.png"),
            },
            {
            url: require("@/assets/img/h1-clients-img-5.png"),
            },
        ],
        };
    },
    };
</script>

<style lang="scss" scoped>

@import '../assets/style/variables.scss';

//Clients Logo

.container-logo{
    padding: 8px 0;
    background-color: $background-clients;
    .clients-box{
    padding: 55px 55px;   
    }
    ul{
        list-style-type: none; 
        li {
            img{
            width: 100%;
            }
        }
    }   
}       

</style>