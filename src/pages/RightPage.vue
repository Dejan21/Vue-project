<template>
    <div class="absolute pt-20 right-96 inline">
        <ul>
         <li v-for="appointment in appointments"
         :key="appointment.id"
         class="mr-6 h-18 border-b border-b-gray"
         >
         <img :src="appointment.defaultAvatar" 
              class="relative right-14 top-12" />
         <span>{{appointment.content}}</span>
         <br />
         <span class="font-bold">{{appointment.pieces}}</span>
         <img :src="appointment.defaultAvatarIcon" class="relative left-44 bottom-10" />
         </li>
        </ul>
    </div>
</template>

<script>
    import Image1Icon from "../assets/image1.png";
    import ImageIcon from "../assets/image.png";
    import ArrowSquareRightIcon from "../assets/ArrowSquareRight.png";
    import { ref } from 'vue'

 export default {
    setup(){
      const appointments = ref([
        {
                 id: 1,
                 content:'New clients',
                 pieces: '44',
                 defaultAvatarIcon: ArrowSquareRightIcon,
                 defaultAvatar: Image1Icon,
             },
             {
                 id: 2,
                 content:'Appointments booked',
                 pieces: '26',
                 defaultAvatar: ImageIcon,
                 defaultAvatarIcon: ArrowSquareRightIcon,
             },
             {
                 id: 3,
                 content:'Appointments booked',
                 pieces: '8',
                 defaultAvatar: ImageIcon,
                 defaultAvatarIcon: ArrowSquareRightIcon,
             },
             {
                id: 4,
                content:'Appointments booked',
                pieces: '6',
                defaultAvatar: ImageIcon,
                defaultAvatarIcon: ArrowSquareRightIcon,
             },
      ])
        return {
         appointments
        }
    }
 }
</script>

<style>
 /* li{
    border-bottom: 1px solid grey;
 } */
</style>