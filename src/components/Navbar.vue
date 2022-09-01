<template>
  <div class="mt-5 border-solid shadow-md navbar bg-white-500 p-4 w-30 flex flex-row justify-between md:flex">
    <p class="text-left pl-72 font-bold text-gray-500 text-lg">Home</p>
    <div class="flex font-bold items-center ml-56">
      <img src="../assets/Grouplogo.png"  />
      <h1>Sellsio</h1>
    </div>
    <div class="input flex pr-36">
      <img src="../assets/Search.png" class="mt-2 absolute right-80 top-8 pr-2" />
      <input
       type="text" 
       placeholder="Search for a client" 
       class="rounded-lg border-solid border-2 w-72 h-8 mr-40 input pl-2" />
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

<style>
  .input{
    border-color: rgba(247, 144, 137, 1);
  }
</style>