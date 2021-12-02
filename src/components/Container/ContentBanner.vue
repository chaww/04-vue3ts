<template>
  <div class="content-wrapper-header">
    <div class="content-wrapper-context">
      <h3 class="img-content">
        <svg viewBox="0 0 512 512">
          <path
            d="M467 0H45C20.099 0 0 20.099 0 45v422c0 24.901 20.099 45 45 45h422c24.901 0 45-20.099 45-45V45c0-24.901-20.099-45-45-45z"
            fill="#d6355b"
            data-original="#ff468c"
          />
          <path
            xmlns="http://www.w3.org/2000/svg"
            d="M512 45v422c0 24.901-20.099 45-45 45H256V0h211c24.901 0 45 20.099 45 45z"
            fill="#d6355b"
            data-original="#d72878"
          />
          <path
            xmlns="http://www.w3.org/2000/svg"
            d="M467 30H45c-8.401 0-15 6.599-15 15v422c0 8.401 6.599 15 15 15h422c8.401 0 15-6.599 15-15V45c0-8.401-6.599-15-15-15z"
            fill="#2e000a"
            data-original="#700029"
          />
          <path
            xmlns="http://www.w3.org/2000/svg"
            d="M482 45v422c0 8.401-6.599 15-15 15H256V30h211c8.401 0 15 6.599 15 15z"
            fill="#2e000a"
            data-original="#4d0e06"
          />
          <path
            xmlns="http://www.w3.org/2000/svg"
            d="M181 391c-41.353 0-75-33.647-75-75 0-8.291 6.709-15 15-15s15 6.709 15 15c0 24.814 20.186 45 45 45s45-20.186 45-45-20.186-45-45-45c-41.353 0-75-33.647-75-75s33.647-75 75-75 75 33.647 75 75c0 8.291-6.709 15-15 15s-15-6.709-15-15c0-24.814-20.186-45-45-45s-45 20.186-45 45 20.186 45 45 45c41.353 0 75 33.647 75 75s-33.647 75-75 75z"
            fill="#d6355b"
            data-original="#ff468c"
          />
          <path
            xmlns="http://www.w3.org/2000/svg"
            d="M391 361h-30c-8.276 0-15-6.724-15-15V211h45c8.291 0 15-6.709 15-15s-6.709-15-15-15h-45v-45c0-8.291-6.709-15-15-15s-15 6.709-15 15v45h-15c-8.291 0-15 6.709-15 15s6.709 15 15 15h15v135c0 24.814 20.186 45 45 45h30c8.291 0 15-6.709 15-15s-6.709-15-15-15z"
            fill="#d6355b"
            data-original="#d72878"
          />
        </svg>
        Adobe Stock
      </h3>
      <div class="content-text">
        Grab yourself 10 free images from Adobe Stock in a 30-day free trial
        plan and find perfect image, that will help you with your new project.
      </div>
      <button class="content-button">Start free trial</button>
    </div>
    <img
      class="content-wrapper-img"
      src="https://assets.codepen.io/3364143/glass.png"
      alt=""
    />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  setup() {
    return {};
  },
});
</script>

<style lang="scss">
.content-wrapper-header {
  display: flex;
  align-items: center;
  width: 100%;
  justify-content: space-between;
  background-image: url("https://www.transparenttextures.com/patterns/cubes.png"),
    linear-gradient(
      to right top,
      #cf4af3,
      #e73bd7,
      #f631bc,
      #fd31a2,
      #ff3a8b,
      #ff4b78,
      #ff5e68,
      #ff705c,
      #ff8c51,
      #ffaa49,
      #ffc848,
      #ffe652
    );
  border-radius: 14px;
  padding: 20px 40px;
  @media screen and (max-width: 415px) {
    padding: 20px;
  }
}

.content-wrapper-context {
  max-width: 350px;
}

.img-content {
  font-weight: 500;
  font-size: 17px;
  display: flex;
  align-items: center;
  margin: 0;
  svg {
    width: 28px;
    margin-right: 14px;
  }
}

.content-text {
  font-weight: 400;
  font-size: 14px;
  margin-top: 16px;
  line-height: 1.7em;
  color: #ebecec;
  display: -webkit-box;
  -webkit-line-clamp: 4;
  -webkit-box-orient: vertical;
  overflow: hidden;
  text-overflow: ellipsis;
}

.content-button {
  background-color: #3a6df0;
  border: none;
  padding: 8px 26px;
  color: #fff;
  border-radius: 20px;
  margin-top: 16px;
  cursor: pointer;
  transition: 0.3s;
  white-space: nowrap;
}

.content-wrapper-img {
  width: 186px;
  object-fit: cover;
  margin-top: -25px;
  object-position: center;
  @media screen and (max-width: 570px) {
    width: 110px;
  }
}
</style>
