<!-- eslint-disable vue/multi-word-component-names -->
<template>
  <div class="mt-5 navbar bg-red-500 p-4 w-30 flex flex-row">
    <p class="text-left pl-3">Home</p>
    <div class="h1">
      <img src="../assets/Vector.png" alt="" />
      <h1>Sellsio</h1>
    </div>
    <div class="input">
      <input type="text" placeholder="search for a client" class="ml-30" />
    </div>
  </div>
</template>

<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Navbar",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
.h1 {
  margin-left: 690px;
  font-size: large;
  color: black;
}
input {
  margin-left: 700px;
}
.navbar {
  background-color: rgb(197, 181, 181);
  box-shadow: 20px;
}
</style>
