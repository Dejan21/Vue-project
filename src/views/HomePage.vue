<template>
  <div class="home">
    <Navbar msg="Home" />
    <HeaderComponent msg="Home" />
  </div>
  <div>
  <img src="../assets/Frame.png" class="m-auto mt-10">
    <ul >
      <li 
      v-for="client in clients" 
      :key="client.id" 
      class=" li bg-red-50 p-2 "
      >
        <span>{{client.name}}</span>
        <span>{{client.number}}</span>
        <span>{{client.description}}</span>
        <button>
         <img src="../assets/Reply.png">
        </button>
      </li>
    </ul>
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import Navbar from "../components/Navbar.vue";
import HeaderComponent from "@/components/HeaderComponent.vue";

export default {
  components: {
    Navbar,
    HeaderComponent
},
data(){
  return {
    clients: [
      {
        id:1,
        name: 'Michael Connor',
        number: '+ 41 34 345 2033',
        description: 'Hey Dr. Richard, I’m trying to reach out this whole morning, but it seems you and your staff are too busy to answer me on my SMS. Please, I’m waiting here for your response. Have a nice day, Michael!',
      },
      {
        id:1,
        name: 'Amanda',
        number: '+ 41 12 585 2236',
        description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
      },
      {
        id:1,
        name: 'John Connor',
        number: '+41 34 345 2023',
        description: 'Hey Dr. Richard, I’m trying to reach out this whole morning, but it seems you and your staff are too busy to answer me on my SMS. Please, I’m waiting here for your response. Have a nice day, Michael!',
      },
      {
        id:1,
        name: 'Helen Connor',
        number: '+41 32 25 5889',
        description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
      },
      {
        id:1,
        name: 'Michael Connor',
        img: '../assets/Reply.png',
        number: '+41 34 345 2023',
        description: 'Hey Dr. Richard, I’m trying to reach out this whole morning, but it seems you and your staff are too busy to answer me on my SMS. Please, I’m waiting here for your response. Have a nice day, Michael!',
      },
       {
        id:1,
        name: 'Michael Connor',
        number: '+41 34 345 2023',
        description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
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
    height: 200px;
}

</style>