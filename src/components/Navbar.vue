<template>
  <div class="mt-5 border-solid shadow-md navbar bg-white-500 p-4 w-30 flex flex-row justify-between">
    <p class="text-left pl-3">Home</p>
    <div class="flex font-bold items-center">
      <img src="../assets/Grouplogo.png"  />
      <h1>Sellsio</h1>
    </div>
    <div class="input flex  border-red-300">
      <img src="../assets/Search.png" class="mt-2 fixed right-7 top-8" />
      <input
       v-model="newClientName"
       type="text" 
       placeholder="Search for a client" 
       class="ml-30 rounded-lg border-red-300 w-72 h-8 " />
    </div>
  </div>
</template>

<script>
export default {
  name: "NavbarComponent",
  props: {
    msg: String,
  },
  data(){
    return {
    
    }
  }
};
</script>


