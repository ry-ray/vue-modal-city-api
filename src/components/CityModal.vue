<template>
  <div class="modal__city-box">
    <div class="modal__city-esc">
      <div class="modal__city-x">
        <svg
          id="x-1"
          width="18"
          height="18"
          viewBox="0 0 18 18"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M1.45312 16.5469L16.5469 1.45337"
            stroke="white"
            stroke-width="2"
            stroke-linecap="round"
          />
        </svg>
        <svg
          id="x-2"
          width="18"
          height="18"
          viewBox="0 0 18 18"
          fill="none"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M1.45325 1.45312L16.5468 16.5469"
            stroke="white"
            stroke-width="2"
            stroke-linecap="round"
          />
        </svg>
      </div>
    </div>
    <h2 class="modal__city-title">Выберите город</h2>
    <input class="modal__city-input" type="text" />
  </div>
</template>

<script>
export default {
  name: "CityModal",
};
</script>

<style scoped lang="scss">
.modal__city-box {
  position: absolute;
  display: flex;
  width: 570px;
  top: 50px;
  bottom: 50px;
  left: 50%;
  transform: translateX(-50%);
  flex-direction: column;
  // background: #FFFFFF;
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

.modal__city-esc {
  position: absolute;
  width: 40px;
  height: 40px;
  right: -70px;
  top: 0px;
  background: #65c6a2;
  border-radius: 50%;

  cursor: pointer;
  @media (max-width: 570px) {
    position: absolute;
    right: 10px;
    top: 10px;
    background-color: #65c6a2;
  }
}

.modal__city-x {
  position: absolute;
  left: 20px;
  top: 20px;
}

#x-2 {
  position: absolute;
  left: -7.55px;
  top: -7.55px;
}

#x-1 {
  position: absolute;
  left: -7.55px;
  top: -7.55px;
}

.modal__city-title {
  position: absolute;
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

.modal__city-input {
  position: absolute;
  width: 430.09px;
  height: 56px;
  left: 70px;
  top: 120px;
}
</style>
