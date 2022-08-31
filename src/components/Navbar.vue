<template>
  <div class="mt-5 border-solid shadow-md navbar bg-white-500 p-4 w-30 flex flex-row justify-between">
    <p class="text-left pl-64 text-slate-600 text-lg">Home</p>
    <div class="flex font-bold items-center">
      <img src="../assets/Grouplogo.png"  />
      <h1>Sellsio</h1>
    </div>
    <div class="input flex pr-48">
      <img src="../assets/Search.png" class="mt-2 absolute  right-96 top-8" />
      <input
       type="text" 
       placeholder="Search for a client" 
       class="rounded-lg border-solid border-2 border-red-300 w-72 h-8 mr-40" />
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


