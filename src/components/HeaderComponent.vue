<template>
<div class="container-md m-auto flex flex-row justify-between h-10 gap-8 max-w-2xl mt-2 ">
 <div class="flex  container-fluid absolute left-px gap-8 pl-40  bg-white border-x-2 border-b-2  border-red-300 rounded-lg">
  <div>
        <img src="../assets/home.png" class="h-20 w-30  m" >
    </div>
    <div>
        <img src="../assets/Calendar.png" class="h-20 w-30 " >
    </div>
    <div>
        <img src="..//assets/Shifts.png" class="h-20 w-30 " >
    </div>
    <div>
        <img src="../assets/Clients.png" class="h-20 w-30 " >
    </div>
    <div>
        <img src="../assets/Invoices.png" class="h-20 w-30 " >
    </div>
    <div>
        <img src="../assets/SmsCampaign.png" class="h-20 w-30 " >
    </div>
    <div>
        <img src="../assets/Forms.png" class="h-20 w-30 " >
    </div>
    <div  >
        <img src="../assets/Admin.png" class="h-20 w-30 " >
    </div>
    <div>
        <img src="../assets/Profile.png" class="w-30 " >
   </div>
 </div>
</div>
</template>

<script>
export default {
  name: "HeaderComponent",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
 .container-fluid{
  margin-left: 190px;
  padding: 10px
 }
</style>