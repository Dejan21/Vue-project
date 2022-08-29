<template>
    <div class="absolute pt-32 right-96 inline">
        <ul>
         <li v-for="appointment in appointments"
         :key="appointment.id"
         class="p-2"
         >
         <span>{{appointment.content}}</span>
         <br />
         <span class="font-bold">{{appointment.pieces}}</span>
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
            },
            {
                id: 2,
                content:'Appointments booked',
                pieces: '26',
            },
            {
                id: 3,
                content:'Appointments booked',
                pieces: '8',
            },
            {
                id: 4,
                content:'Appointments booked',
                pieces: '6',
            },
            ]
        }
    }
 }
</script>

<style>

</style>