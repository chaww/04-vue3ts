<template>
  <header class="header">
    <HeaderMenu />
    <SearchBar />
    <HeaderUser />
  </header>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import HeaderMenu from "@/components/Header/HeaderMenu.vue";
import SearchBar from "@/components/Header/SearchBar.vue";
import HeaderUser from "@/components/Header/HeaderUser.vue";

export default defineComponent({
  components: { HeaderMenu, SearchBar, HeaderUser },
  setup() {
    return {};
  },
});
</script>

<style lang="scss">
.header {
  display: flex;
  align-items: center;
  flex-shrink: 0;
  height: 50px;
  width: 100%;
  border-bottom: 1px solid var(--border-color);
  white-space: nowrap;
}
</style>
