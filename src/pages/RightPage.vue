<template>
    <div class="absolute pt-16 right-96 inline">
        <ul>
         <li v-for="appointment in appointments"
         :key="appointment.id"
         class="p-2"
         >
         <img :src="appointment.image" 
              class="relative right-14 top-12" />
         <span>{{appointment.content}}</span>
         <br />
         <span class="font-bold">{{appointment.pieces}}</span>
         <img :src="appointment.img" class="relative left-44 bottom-10" />
         </li>
        </ul>
    </div>
</template>

<script>
 export default {
    data(){
        return {
            appointments: [
             {
                id: 1,
                content:'New clients',
                pieces: '44',
                image: [require("../assets/image.png")],
                img: [require("../assets/ArrowSquareRight.png")]
            },
            {
                id: 2,
                content:'Appointments booked',
                pieces: '26',
                image: [require("../assets/image1.png")],
                img: [require("../assets/ArrowSquareRight.png")]
            },
            {
                id: 3,
                content:'Appointments booked',
                pieces: '8',
                image: [require("../assets/image1.png")],
                img: [require("../assets/ArrowSquareRight.png")]
            },
            {
                id: 4,
                content:'Appointments booked',
                pieces: '6',
                image: [require("../assets/image1.png")],
                img: [require("../assets/ArrowSquareRight.png")]
            },
            ]
        }
    }
 }
</script>

<style>

</style>