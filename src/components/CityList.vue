<template>
  <div class="modal__city-list">
    <div v-for="city in cities" :key="cities.indexOf(city)">
      <p class="modal__city-list-item">
        {{ city }}
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      cities: ["Екатеринбург", "Москва", "Санкт-Петербург", "Пермь", "Омск"],
    };
  },
  // props:{
  //   cities:{
  //     type: String,
  //     required: true,
  //   }
  // },
  
};
</script>

<style lang="scss">
.modal__city-list {
  overflow-y: auto;
}
.modal__city-list-item {
  margin: 15px 0px;
  text-align: start;
}
</style>
