<template>
<div class="container-md h-10 flex flex-row m-4 ">
 <div class="flex container-fluid absolute left-24 gap-8  w-4/6 bg-white border-x-2 border-b-2  border-red-300 rounded-lg">
  <div>
        <img src="../assets/home.png" class="h-20 w-30 ml-8 pb-2" >
    </div>
    <div>
        <img src="../assets/Calendar.png" class="h-18 w-30" >
    </div>
    <div>
        <img src="..//assets/Shifts.png" class="h-18 w-30" >
    </div>
    <div>
        <img src="../assets/Clients.png" class="h-18 w-30" >
    </div>
    <div>
        <img src="../assets/Invoices.png" class="h-18 w-30" >
    </div>
    <div>
        <img src="../assets/SmsCampaign.png" class="h-18 w-30" >
    </div>
    <div>
        <img src="../assets/Forms.png" class="h-18 w-30 " >
    </div>
    <div  >
        <img src="../assets/Admin.png" class="h-18 w-30 " >
    </div>
    <div>
        <img src="../assets/Profile.png" class="w-30 h-30 top-px absolute" >
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
  padding: 10px;
  border-color: rgba(241, 183, 179, 0), rgba(216, 89, 78, 1), rgba(255, 255, 255, 0.9)
 }

</style>