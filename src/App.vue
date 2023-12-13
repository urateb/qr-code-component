<template>
  <div class="qr-code__card">
    <img src="./assets/images/image-qr-code.png" class="qr-code__image" />
    <div class="qr-code__card--title">Improve your front-end skills by building projects</div>
    <div class="qr-code__card--description">Scan the QR code to visit Frontend Mentor and take your coding skills to the
      next level</div>
  </div>
</template>

<script>
import './assets/styles/main.scss'
export default {
  name: 'App',
}
</script>

<style lang="scss">
#app {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}

.qr-code {
  &__card {
    background-color: hsl(0, 0%, 100%);
    border-radius: 16px;
    width: 80%;
    padding: 16px;
    display: flex;
    flex-direction: column;
    box-shadow: 6px 8px 11px 1px hsla(218, 44%, 22%, 0.1);

    &--title {
      font-weight: 700;
      text-align: center;
      font-size: 21px;
      margin: 30px 20px 20px 20px;
    }

    &--description {
      text-align: center;
      font-size: 15px;
      color: hsl(220, 15%, 55%);
      margin: 0 7px 20px 7px;

    }

    @media (min-width: 768px) {
      width: 20%;
    }
  }

  &__image {
    width: 100%;
    border-radius: 16px;
  }
}
</style>
