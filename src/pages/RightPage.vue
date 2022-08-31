<template>
    <div class="flex flex-col float-right mr-96 mt-24 w-72 h-16">
        <ul >
         <li v-for="appointment in appointments"
         :key="appointment.id"
         class="border border-t-0 border-r-0 border-l-0 h-20 border-b-gray w-72 relative pr-10 text-justify"
         >
         <img :src="appointment.defaultAvatar" 
              class=" relative  top-5" />
         <span class="content relative left-14 bottom-6">{{appointment.content}}</span>
         <br />
         <span class="font-bold relative left-14 bottom-6">{{appointment.pieces}}</span>
         <img :src="appointment.defaultAvatarIcon" class="relative left-64 bottom-16" />
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
 .content{
    color:#9F9F9F
 }
 ul{
    background-color: #FFFCFC;
 }
 
</style>