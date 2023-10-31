<template>
  <!-- 装载是内容 -->
  <div class="xtx-tabs-panel" v-show="activeName === name">
    <slot />
  </div>
</template>
<script>
import { inject } from "vue";
export default {
  name: "XtxTabsPanel",
  props: {
    label: {
      type: String,
      default: "",
    },
    name: {
      type: [String, Number],
      default: "",
    },
  },
  setup() {
    // console.log("213");
    const activeName = inject("activeName");
    return { activeName };
  },
};
</script>
<style scoped lang="scss"></style>
