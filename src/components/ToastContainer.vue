<template>
  <div id="toast-container">
    <toast-card v-for="i in 5" :key="i" />
  </div>
</template>

<script>
import ToastCard from "./ToastCard.vue";

export default {
  components: { ToastCard },
};
</script>

<style lang="scss" scoped>
#toast-container {
  bottom: 0;
  left: 0;
  padding: 10px;
  position: fixed;
  width: fit-content;
  z-index: 50;

  & > * {
    margin: 10px 0;
  }
}
</style>
