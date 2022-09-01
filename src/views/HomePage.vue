<template>
  <Navbar  />

  <div class="home ">
    <HeaderComponent  />
    <LeftPage />
    <RightPage />

  <img src="../assets/Frame.png" class="float-right relative left-5 pt-24 ">
    <ul class="mt-40" >
      <li 
      v-for="client in clients" 
      :key="client.id" 
      class=" li p-1 relative left-19 pl-20 pb-52 text-start border"
      >
        <img :src="client.defaultAvatar" class="relative top-10 right-16" />
        
        <span class="first relative bottom-7"> {{ client.name }} </span>
        <span class="first relative bottom-7">{{ client.number }}</span>
        <span class="relative float-right first bottom-7 ">{{ client.hours }}</span>
        <br />
        <span class="relative bottom-7">{{ client.description }}</span>
        <button class="block">
         <img class="relative bottom-4" src="../assets/Reply.png">
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
import { ref } from 'vue'
import defaultAvatarIcon from "../assets/michael.png";
import defaultIcon from "../assets/amanda.png";
import AndyIcon from "../assets/Andy.png";
import UserCircle from "../assets/UserCircle.png";
import Helen from "../assets/helen.png";

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
         defaultAvatar: defaultAvatarIcon,
         neededData: {img: defaultAvatarIcon}
       },
       {
         id:1,
         name: 'Amanda Horryngton',
         number: '(+ 41 12 585 2236)',
         hours: '5h ago',
         description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
         defaultAvatar: defaultIcon,
         neededData: {img: defaultAvatarIcon}
       },
       {
         id:1,
         name: 'John McRowe',
         number: '(+41 34 345 2023)',
         hours: '6h ago',
         description: 'Hey Dr. Richard, I’m trying to reach out this whole morning, but it seems you and your staff are too busy to answer me on my SMS. Please, I’m waiting here for your response. Have a nice day, Michael!',
         defaultAvatar: UserCircle,
         neededData: {img: defaultAvatarIcon}
       },
       {
         id:1,
         name: 'Helen Wisemeyer',
         number: '(+41 32 25 5889)',
         hours: '1 day ago',
         description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
         defaultAvatar: Helen,
         neededData: {img: defaultAvatarIcon}
       },
       {
         id:1,
         name: 'Michael Connor',
         number: '(+41 34 345 2023)',
         hours: '2 days ago',
         description: 'Hey Dr. Richard, I’m trying to reach out this whole morning, but it seems you and your staff are too busy to answer me on my SMS. Please, I’m waiting here for your response. Have a nice day, Michael!',
         defaultAvatar: UserCircle,
         neededData: {img: defaultAvatarIcon}
       },
        {
         id:1,
         name: 'Andy Stockton',
         number: '(+41 34 345 2023)',
         hours: '5h ago',
         description: 'Hey, guys! Thanks for your time and effort. I wll definitely recommend it to anybody else.',
         defaultAvatar: AndyIcon,
         neededData: {img: defaultAvatarIcon}
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
    width: 605px;
    height: 151px;
    margin-left: 640px;
    border-bottom: 1px solid rgba(224, 224, 224, 1);
    border-left: 1px solid rgba(224, 224, 224, 1);
    border-right: 1px solid rgba(224, 224, 224, 1);
    background-color: #FFFCFC;
}

.first{
  color:#9F9F9F;
}
.home{
  background-color: #FFFCFC;
}

</style>