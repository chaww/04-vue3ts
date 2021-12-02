<template>
  <div class="content-wrapper">
    <ContentBanner />
    <ContentInstall />
    <ContentPlan />
  </div>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import ContentBanner from "@/components/Container/ContentBanner.vue";
import ContentInstall from "@/components/Container/ContentInstall.vue";
import ContentPlan from "@/components/Container/ContentPlan.vue";

export default defineComponent({
  components: { ContentBanner, ContentInstall, ContentPlan },
  setup() {
    return {};
  },
});
</script>

<style lang="scss">
.content-wrapper {
  display: flex;
  flex-direction: column;
  color: var(--theme-color);
  padding: 20px 40px;
  height: 100%;
  overflow: auto;
  background-color: var(--theme-bg-color);
  @media screen and (max-width: 510px) {
    padding: 20px;
  }
  &.overlay {
    pointer-events: none;
    transition: 0.3s;
    background-color: var(--overlay-bg);
  }
}
</style>
