<template>
  <div class="mt-5 border-solid shadow-md navbar bg-white-500 p-4 w-30 flex flex-row justify-between">
    <p class="text-left pl-3">Home</p>
    <div class="flex font-bold items-center">
      <img src="../assets/Grouplogo.png"  />
      <h1>Sellsio</h1>
    </div>
    <div class="input flex">
      <img src="../assets/Search.png" class="mt-2" />
      <input type="text" placeholder="search for a client" class="ml-30" />
    </div>
  </div>
</template>

<script>
export default {
  name: "NavbarComponent",
  props: {
    msg: String,
  },
};
</script>


