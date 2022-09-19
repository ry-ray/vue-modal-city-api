<template>
  <input 
      class="modal__city-input modal__city-text"
      type="text"
      placeholder="ваш город"
      
    />
</template>

<script>
export default {
}
</script>

<style lang="scss">

input::-webkit-input-placeholder {color:#ded9f8}
input:-moz-placeholder {color:#ded9f8}


.modal__city-input {
  height: 56px;
  margin: 30px 0px;
  padding: 13.5px 25px;
  box-sizing: border-box;

  border: 1px solid #ded9f8;
  border-radius: 5px;
}


</style>