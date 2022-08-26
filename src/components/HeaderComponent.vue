<template>
<div class="container-md m-auto flex flex-row justify-between h-10 gap-8 max-w-2xl mt-2">
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
</template>

<script>
export default {
  name: "HeaderComponent",
  props: {
    msg: String,
  },
};
</script>
