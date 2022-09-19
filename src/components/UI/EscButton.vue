<template>
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
</template>

<script>
export default {

}
</script>

<style lang="scss">
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

</style>