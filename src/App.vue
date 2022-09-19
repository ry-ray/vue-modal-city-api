<template>
  <CityModal />
</template>

<script>
import CityModal from "./components/CityModal.vue";

export default {
  name: "App",
  components: {
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
