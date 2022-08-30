<template>
  <div class="home">
    <Navbar  />
    <HeaderComponent  />
    <LeftPage />
    <RightPage />
  </div>
  <div class="bg-red-50 ">
  <img src="../assets/Frame.png" class="m-auto mt-12 pt-12">
    <ol class="" >
      <li 
      v-for="client in clients" 
      :key="client.id" 
      class=" li bg-red-50 p-2 relative left-14 text-start border-double"
      >
        <img :src="client.image" class="relative top-24 right-16" />
        <span > {{ client.name }} </span>
        <span>{{ client.number }}</span>
        <span class="relative left-20 ">{{ client.hours }}</span>
        <br />
        <br />
        <span>{{ client.description }}</span>
        <button class="block">
         <img src="../assets/Reply.png">
        </button>
      </li>
    </ol>
  </div>
</template>

<script>

import Navbar from "../components/Navbar.vue";
import HeaderComponent from "@/components/HeaderComponent.vue";
import LeftPage from "@/pages/LeftPage.vue";
import RightPage from "@/pages/RightPage.vue";
import { ref } from 'vue'

export default {
  components: {
    Navbar,
    HeaderComponent,
    LeftPage,
    RightPage
},
setup(){

  const clients = ref ([
    {
         id:1,
         name: 'Michael Connor',
         number: '(+ 41 34 345 2033)',
         hours: '2h ago',
         description: 'Hey Dr. Richard, I’m trying to reach out this whole morning, but it seems you and your staff are too busy to answer me on my SMS. Please, I’m waiting   here       for your response. Have a nice day, Michael!',
         image: [require("../assets/michael.png")],
       },
       {
         id:1,
         name: 'Amanda',
         number: '(+ 41 12 585 2236)',
         hours: '5h ago',
         description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
         image: [require("../assets/amanda.png")],
       },
       {
         id:1,
         name: 'John Connor',
         number: '(+41 34 345 2023)',
         hours: '6h ago',
         description: 'Hey Dr. Richard, I’m trying to reach out this whole morning, but it seems you and your staff are too busy to answer me on my SMS. Please, I’m waiting here for your response. Have a nice day, Michael!',
         image: [require("../assets/UserCircle.png")],
       },
       {
         id:1,
         name: 'Helen Connor',
         number: '(+41 32 25 5889)',
         hours: '1 day ago',
         description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
         image: [require("../assets/helen.png")],
       },
       {
         id:1,
         name: 'Michael Connor',
         number: '(+41 34 345 2023)',
         hours: '2 days ago',
         description: 'Hey Dr. Richard, I’m trying to reach out this whole morning, but it seems you and your staff are too busy to answer me on my SMS. Please, I’m waiting here for your response. Have a nice day, Michael!',
         image: [require("../assets/UserCircle.png")],
       },
        {
         id:1,
         name: 'Michael Connor',
         number: '(+41 34 345 2023)',
         hours: '5h ago',
         description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
         image: [require("../assets/michael.png")],
       },
  ])
  return {
  clients
  }
}
};
</script>

<style scoped>
.li{
    width: 590px;
    margin-top: 2px;
    height: 270px;
    border: double;
    text-align: start;
    padding-left: 80px;
    margin-left: 600px;
}

</style>