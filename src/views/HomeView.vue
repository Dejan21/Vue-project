<template>
  <div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png" /> -->
    <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
    <Navbar msg="Home" />
    <Header msg="Home" />
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";
import Navbar from "../components/Navbar.vue";
import Header from "../components/Header.vue";

export default {
  name: "HomeView",
  components: {
    Navbar,
    Header,
  },
};
</script>
