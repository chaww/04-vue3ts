<template>
  <div class="header-menu">
    <a class="menu-link active" href="#">Apps</a>
    <a class="menu-link notify" href="#">Your work</a>
    <a class="menu-link" href="#">Discover</a>
    <a class="menu-link notify" href="#">Market</a>
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
.header-menu {
  display: flex;
  align-items: center;
  height: 100%;
  a {
    display: flex;
    align-items: center;
    height: 100%;
    padding: 0 30px;
    text-decoration: none;
    color: var(--inactive-color);
    border-bottom: 2px solid transparent;
    transition: 0.3s;
    position: relative;
    &::after {
      content: "";
      bottom: 0;
      left: 0;
      right: 0;
      top: 0;
      transition: 0.3s;
      height: 100%;
      width: 100%;
      position: absolute;
      border-bottom: 2px solid transparent;
    }
    &.active,
    &:hover {
      color: var(--theme-color);
      &:after {
        border-bottom: 2px solid var(--theme-color);
      }
    }
  }
}

.notify {
  position: relative;
  &:before {
    content: "";
    position: absolute;
    background-color: #3a6df0;
    width: 6px;
    height: 6px;
    border-radius: 50%;
    right: 20px;
    top: 16px;
  }
  @media screen and (max-width: 1055px) {
    display: none;
  }
}
</style>
