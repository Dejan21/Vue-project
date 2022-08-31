<template>
    <div class="absolute pt-24 ml-72">
        <ul class="border-b-gray w-72">
         <li  v-for="sale in sales"
              :key="sale.id" 
              class=" pt-6 h-20 border border-t-0 border-l-0 border-r-0 pl-20 text-justify w-72 border-b-gray"
         >
           <span class="content relative right-6"> {{sale.content}} </span>
           <br />
           <span class="font-bold relative right-6"> {{sale.pieces}} </span>
           <span class="font-bold relative right-6"> {{sale.price}} </span>
           <img :src="sale.defaultAvatar" 
                 class="relative right-20 text-start bottom-12" 
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
    margin-left: 52px;
    background-color: #FFFCFC;
 }
 .content {
    color: #9F9F9F
 }
 
</style>