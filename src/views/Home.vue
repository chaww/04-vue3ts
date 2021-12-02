<template>
  <div class="app-wrapper">
    <div class="app">
      <Header />
      <div class="wrapper">
        <LeftSide />
        <Container />
      </div>
    </div>
    <Popup />
    <!-- <div class="overlay-app active"></div> -->
    <div class="overlay-app"></div>
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Header from "@/components/Header/Header.vue";
import LeftSide from "@/components/LeftSide/LeftSide.vue";
import Container from "@/components/Container/Container.vue";
import Popup from "@/components/Container/Popup.vue";

export default defineComponent({
  components: { Header, LeftSide, Container, Popup },
  setup() {
    return {};
  },
});
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Poppins:wght@200;300;400;500;600;700&display=swap");

* {
  outline: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  padding: 0;
  margin: 0;
  font-family: "Poppins", sans-serif;
}

:root {
  --theme-bg-color: rgba(16, 18, 27, 40%);
  --theme-deep-color: rgba(16, 18, 27, 40%);
  --border-color: rgba(113, 119, 144, 25%);
  --theme-color: #f9fafb;
  --inactive-color: rgb(113, 119, 144, 78%);
  --hover-menu-bg: rgba(12, 15, 25, 30%);
  --content-title-color: #999ba5;
  --content-bg: rgb(146, 151, 179, 13%);
  --button-inactive: rgb(249, 250, 251, 55%);
  --popup-bg: rgb(22, 25, 37);
  --overlay-bg: rgba(36, 39, 59, 0.3);
}

.app-wrapper {
  background-image: url(https://4kwallpapers.com/images/wallpapers/macos-big-sur-apple-layers-fluidic-colorful-dark-wwdc-2020-5120x2880-1432.jpg);
  background-size: cover;
  background-position: center;
}
.app {
  background-color: var(--theme-bg-color);
  /* height: 100vh; */
  width: 100vw;
  overflow: hidden;
  font-size: 15px;
  font-weight: 500;
  position: relative;
  backdrop-filter: blur(20px);
  -webkit-backdrop-filter: blur(20px);
}
.wrapper {
  display: flex;
  flex-grow: 1;
  overflow: hidden;
}

.overlay-app {
  width: 100%;
  height: 100%;
  position: fixed;
  left: 0;
  top: 0;
  pointer-events: all;
  background-color: rgba(36, 39, 59, 0.8);
  opacity: 0;
  visibility: hidden;
  transition: 0.3s;
  &.active {
    visibility: visible;
    opacity: 1;
  }
}
</style>
