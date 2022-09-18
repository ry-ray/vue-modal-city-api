<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
  <CityModal />
  <!-- <HelloWorld msg="Welcome to Your Vue.js App" /> -->
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
import CityModal from "./components/CityModal.vue";

export default {
  name: "App",
  components: {
    // HelloWorld,
    CityModal,
  },
};
</script>

<style lang="scss">
#app {
  display: flex;
  font-family: "Inter", sans-serif;
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 156%;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #212121;
}
</style>
