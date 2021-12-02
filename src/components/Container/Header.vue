<template>
  <div class="main-header">
    <a class="menu-link-main" href="#">All Apps</a>
    <div class="header-menu">
      <a class="main-header-link active" href="#">Desktop</a>
      <a class="main-header-link" href="#">Mobile</a>
      <a class="main-header-link" href="#">Web</a>
    </div>
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
.main-header {
  display: flex;
  align-items: center;
  border-bottom: 1px solid var(--border-color);
  height: 58px;
  flex-shrink: 0;
  .header-menu {
    margin-left: 150px;
    @media screen and (max-width: 1055px) {
      margin: auto;
    }
    a {
      padding: 20px 24px;
    }
  }
}
.menu-link-main {
  text-decoration: none;
  color: var(--theme-color);
  padding: 0 30px;
  @media screen and (max-width: 1055px) {
    display: none;
  }
}
</style>
