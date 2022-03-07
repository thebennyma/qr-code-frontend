<template>
  <div class="qr-code">
    <qrcode-vue
      class="qr-code_component"
      :value="value"
      :foreground="foreground"
      :background="background"
      :size="size"
      level="H"
      :render="render"
    />
    <span class="qr-code_first-spam"
      >Improve your front-end skills by builgin projects</span
    >
    <span class="qr-code_second-spam"
      >Scan the QR code to visit Frontend Mentor and take your coding skills to
      the next level</span
    >
  </div>
</template>

<script>
import QrcodeVue from "qrcode.vue";

export default {
  name: "px-qr-code",
  components: {},
  data() {
    return {
      value: "https://www.frontendmentor.io/challenges",
      foreground: "#ffffff",
      background: "#13a3fb",
      size: 200,
      render: "svg",
    };
  },
  components: {
    QrcodeVue,
  },
};
</script>

<style lang="scss" scoped>
.qr-code {
  display: grid;
  grid-row-gap: 1rem;
  align-items: center;
  justify-items: center;
  text-align: center;
  padding: 1.5rem;
  border-radius: 1rem;
  box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
  background: white;

  &_component {
    background: #13a3fb;
    padding: 2rem;
    border-radius: 1rem;
  }
  &_first-spam,
  &_second-spam {
    font-size: 15px;
    font-family: "Outfit", sans-serif;
  }
  &_first-spam {
    font-weight: 700;
    color: hsl(218, 44%, 22%);
  }

  &_second-spam {
    font-weight: 400;
    color: hsl(220, 15%, 55%);
  }
}
</style>
