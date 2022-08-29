<template>
  <div class="home">
    <Navbar  />
    <HeaderComponent  />
    <LeftPage />
    <RightPage />
  </div>
  <div class="bg-red-50">
  <img src="../assets/Frame.png" class="m-auto mt-12">
    <ul >
      <li 
      v-for="client in clients" 
      :key="client.id" 
      class=" li bg-red-50 p-2 relative left-14 text-start "
      >
        <img :src="client.image" class="relative top-28 right-16" />
        <span> {{ client.name }} </span>
        <span>{{ client.number }}</span>
        <br />
        <br />
        <span>{{ client.description }}</span>
        <button>
         <img src="../assets/Reply.png">
        </button>
      </li>
    </ul>
  </div>
</template>

<script>

import Navbar from "../components/Navbar.vue";
import HeaderComponent from "@/components/HeaderComponent.vue";
import LeftPage from "@/pages/LeftPage.vue";
import RightPage from "@/pages/RightPage.vue";

export default {
  components: {
    Navbar,
    HeaderComponent,
    LeftPage,
    RightPage
},
data(){
  return {
    clients: [
      {
        id:1,
        name: 'Michael Connor',
        number: '(+ 41 34 345 2033)',
        description: 'Hey Dr. Richard, I’m trying to reach out this whole morning, but it seems you and your staff are too busy to answer me on my SMS. Please, I’m waiting here for your response. Have a nice day, Michael!',
        image: [require("../assets/michael.png")],
      },
      {
        id:1,
        name: 'Amanda',
        number: '(+ 41 12 585 2236)',
        description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
        image: [require("../assets/amanda.png")],
      },
      {
        id:1,
        name: 'John Connor',
        number: '(+41 34 345 2023)',
        description: 'Hey Dr. Richard, I’m trying to reach out this whole morning, but it seems you and your staff are too busy to answer me on my SMS. Please, I’m waiting here for your response. Have a nice day, Michael!',
        image: [require("../assets/UserCircle.png")],
      },
      {
        id:1,
        name: 'Helen Connor',
        number: '(+41 32 25 5889)',
        description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
        image: [require("../assets/helen.png")],
      },
      {
        id:1,
        name: 'Michael Connor',
        number: '(+41 34 345 2023)',
        description: 'Hey Dr. Richard, I’m trying to reach out this whole morning, but it seems you and your staff are too busy to answer me on my SMS. Please, I’m waiting here for your response. Have a nice day, Michael!',
        image: [require("../assets/UserCircle.png")],
      },
       {
        id:1,
        name: 'Michael Connor',
        number: '(+41 34 345 2023)',
        description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
        image: [require("../assets/michael.png")],
      },
    ]
  }
}
};
</script>

<style scoped>
.li{
    width: 400px;
    margin: auto;
    margin-top: 2px;
    height: 260px;
}

</style>