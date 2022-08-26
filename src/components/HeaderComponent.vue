<template>
<div class="container-md m-auto flex flex-row justify-between h-10 gap-8 max-w-2xl mt-2 p-11 border-red-300">
 <div class="flex mt-0 container-fluid absolute left-px gap-8 pl-40">
  <div>
        <img src="../assets/home.png" class="h-20 w-30 border border-solid m" >
    </div>
    <div>
        <img src="../assets/Calendar.png" class="h-20 w-30 border border-solid" >
    </div>
    <div>
        <img src="..//assets/Shifts.png" class="h-20 w-30 border border-solid" >
    </div>
    <div>
        <img src="../assets/Clients.png" class="h-20 w-30 border border-solid" >
    </div>
    <div>
        <img src="../assets/Invoices.png" class="h-20 w-30 border border-solid" >
    </div>
    <div>
        <img src="../assets/SmsCampaign.png" class="h-20 w-30 border border-solid" >
    </div>
    <div>
        <img src="../assets/Forms.png" class="h-20 w-30 border border-solid" >
    </div>
    <div  >
        <img src="../assets/Admin.png" class="h-20 w-30 border border-solid" >
    </div>
    <div>
        <img src="../assets/Profile.png" class="h-20 w-30 border border-solid" >
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
  border: red 1px outset;
  margin-left: 190px;
  padding: 10px
 }
</style>