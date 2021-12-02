<template>
  <div class="main-container">
    <Header />
    <Content />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Header from "@/components/Container/Header.vue";
import Content from "@/components/Container/Content.vue";

export default defineComponent({
  components: { Header, Content },
  setup() {
    return {};
  },
});
</script>

<style lang="scss">
.main-container {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
}
</style>
