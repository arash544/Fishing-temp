<template>
  <div class="spinner-cart">
    <div class="spin1"></div>
    <div class="spin2"></div>
    <div class="spin3"></div>
  </div>
</template>

<script>
export default {
  name: "Spinners",
  props: ["spin1", "spin2", "spin3"]
};
</script>

<style lang="scss" scoped>
.spinner-cart {
  width: 500px;
  height: 100px;
  display: flex;
  justify-content: center;
  align-items: center;
  @media only screen and (min-width: 1650px) {
    width: 600px;
  }
}
.spin1 {
  background-color: rgb(93, 197, 150);
  height: 15px;
  width: 15px;
  margin: 2px;
  border-radius: 100%;
  display: inline-block;
  animation-name: move;
  animation-duration: 0.6s;
  animation-iteration-count: infinite;
  animation-timing-function: ease-in-out;
  animation-fill-mode: both;
  animation-delay: 0.07s;
}
.spin2 {
  background-color: rgb(93, 197, 150);
  height: 15px;
  width: 15px;
  margin: 2px;
  border-radius: 100%;
  display: inline-block;
  animation-name: move;
  animation-duration: 0.6s;
  animation-iteration-count: infinite;
  animation-timing-function: ease-in-out;
  animation-fill-mode: both;
  animation-delay: 0.14s;
}
.spin3 {
  background-color: rgb(93, 197, 150);
  height: 15px;
  width: 15px;
  margin: 2px;
  border-radius: 100%;
  display: inline-block;
  animation-name: move;
  animation-duration: 0.6s;
  animation-iteration-count: infinite;
  animation-timing-function: ease-in-out;
  animation-fill-mode: both;
  animation-delay: 0.21s;
}
@keyframes move {
  0% {
    transform: scaleY(10px);
  }

  66% {
    transform: translateY(-10px);
  }

  100% {
    transform: translateY(0);
  }
}
</style>