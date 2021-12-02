<template>
  <a href="#">
    <!-- <SvgFile name="refresh" /> -->
    {{ text }}
    <span class="notification-number updates">{{ noti }}</span>
  </a>
</template>

<script lang="ts">
import { defineComponent } from "vue";
// import SvgFile from "@/components/svg/SvgFile.vue";

export default defineComponent({
  // components: { SvgFile },
  props: {
    noti: {
      type: Number,
      required: true,
    },
    text: {
      type: String,
      required: true,
    },
  },
  setup(props) {
    console.log(props.noti);
    return {};
  },
});
</script>

<style scoped></style>
