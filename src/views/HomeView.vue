<template>
  <div class="home">
    <px-qr-code></px-qr-code>
  </div>
</template>

<script>
//https://github.com/scopewu/qrcode.vue
import PxQrCode from "@/components/PxQrCode.vue";

export default {
  name: "HomeView",
  components: { PxQrCode },
  data() {
    return {};
  },
};
</script>

<style lang="scss" scoped>
.home {
  margin: 1rem;
  width: min-content;
  height: min-content;
  justify-self: center;
}
</style>
