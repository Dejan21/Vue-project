<template>
    <div class="absolute pt-32 ml-96">
        <ul class="border-b-gray w-72">
         <li  v-for="sale in sales"
              :key="sale.id" 
              class=" p-6 h-20 border-b w-70 border-b-gray"
         >
           <span class="relative "> {{sale.content}} </span>
           <br />
           <span class="font-bold relative"> {{sale.pieces}} </span>
           <span class="font-bold text-start"> {{sale.price}} </span>
           <img :src="sale.defaultAvatar" 
                 class="relative right-20 text-start bottom-11" 
                 /> 
         </li>
        </ul>
    </div>
</template>

<script>
import defaultAvatarIcon from "../assets/sales.png";
import IncomeIcon from "../assets/income.png";
import InvoiceIcon from "../assets/invoice.png";
import { ref } from 'vue'

 export default {
    setup () {
        const sales = ref ([
            {
                 id: 1,
                 content:'Daily sales',
                 pieces: '6',
                 defaultAvatar: defaultAvatarIcon,
              
             },
             {
                 id: 2,
                 content:'Retail sales',
                 pieces: '6',
                 defaultAvatar: defaultAvatarIcon,
             },
             {
                 id: 3,
                 content:'Daily income',
                 price: '$ 3344',
                 defaultAvatar: IncomeIcon,
             },
             {
                 id: 4,
                 content:'Retail income',
                 price: '$ 825',
                 defaultAvatar: IncomeIcon,
             },
             {
                 id: 5,
                 content:'Invoices raised',
                 price: '$ 259',
                 defaultAvatar: InvoiceIcon,
             },
             {
                 id: 6,
                 content:'Total invoices',
                 pieces: '156',
                 defaultAvatar: InvoiceIcon,
             },
             {
                 id: 7,
                 content:'Expensens submitted',
                 pieces: '34',
                 defaultAvatar: InvoiceIcon,
           }
        ])
      return {
       sales
      }
    }
 }
</script>


<style>
 li {
    text-align: start;
    margin-left: 52px;
    background-color: #FFFCFC;
 }
 
</style>