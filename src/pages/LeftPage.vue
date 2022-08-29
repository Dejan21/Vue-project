<template>
    <div class="absolute pt-32 ml-96">
        <ul>
         <li  v-for="sale in sales"
              :key="sale.id" 
              class="bg-red-50 p-2"
         >
           <span> {{sale.content}} </span>
           <br />
           <span class="font-bold"> {{sale.pieces}} </span>
           <span class="font-bold"> {{sale.price}} </span>
           <img :src="sale.image" 
                 class="relative right-12 bottom-11" 
                 /> 
         </li>
        </ul>
    </div>
</template>

<script>
 export default {
    data () {
        return {
             sales: [
            {
                id: 1,
                content:'Daily sales',
                pieces: '6',
                image: [require("../assets/sales.png")],
            },
            {
                id: 2,
                content:'Retail sales',
                pieces: '6',
                image: [require("../assets/sales.png")],
            },
            {
                id: 3,
                content:'Daily income',
                price: '$ 3344',
                image: [require("../assets/income.png")],
            },
            {
                id: 4,
                content:'Retail income',
                price: '$ 825',
                image: [require("../assets/income.png")],
            },
            {
                id: 5,
                content:'Invoices raised',
                price: '$ 259',
                image: [require("../assets/invoice.png")],
            },
            {
                id: 6,
                content:'Total invoices',
                pieces: '156',
                image: [require("../assets/invoice.png")],
            },
            {
                id: 7,
                content:'Expensens submitted',
                pieces: '34',
                image: [require("../assets/invoice.png")],
            }
        ]
      }
    }
 }
</script>


<style>

</style>