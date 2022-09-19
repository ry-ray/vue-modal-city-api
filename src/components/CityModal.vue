<template>
  <div class="modal__city-box">
    <EscButton/>
    <h2 class="modal__city-title">Выберите город</h2>
    <MyInput 
    v-bind:value="search"
    @input="getCities"/>
    <CityList :cities="cities"/>
  </div>
</template>

<script>
import MyInput from "./UI/MyInput.vue"
import EscButton from "./UI/EscButton.vue";
import CityList from "./CityList.vue";

export default {
  name: "CityModal",
  components:{
    MyInput,
    EscButton,
    CityList,
},
  data(){
    return{
      search: '',
      cities:[],
    }
  },
  methods: {
    getCities(event) {
      this.search = event.target.value;
      // async function getCities(search){
        // await 
        // return [cities]
      // }
      // this.cities = setTimeout(getCities(this.search),500)
    },
  },
};
</script>

<style scoped lang="scss">
.modal__city-box {
  position: absolute;
  display: flex;
  padding: 60px 70px;
  width: 570px;
  top: 50px;
  bottom: 50px;
  left: 50%;
  transform: translateX(-50%);
  flex-direction: column;
  border-radius: 10px;
  box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.15);
  @media (max-width: 570px) {
    top: 10px;
    bottom: 10px;
    left: 10px;
    right: 10px;
    transform: none;
    width: auto;
  }
}


.modal__city-title {
  display: flex;
  width: 270px;
  height: 30px;
  left: 70px;
  top: 60px;

  font-weight: 600;
  font-size: 20px;
  line-height: 150%;

  color: #5e50a2;
}

.modal__city-text {
  font-family: "Inter";
  font-style: normal;
  font-weight: 400;
  font-size: 18px;
  line-height: 156%;

  color: #212121;
}


</style>
