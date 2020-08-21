<template>
  <div class="wrapper">
    <Spinners />
    <Spinners />
    <Spinners />
    <Spinners />
    <Spinners />
    <Spinners />
  </div>
</template>

<script>
import Spinners from "./Spinners";
export default {
  name: "Loader",
  components: {
    Spinners
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  margin-top: 120px;
  width: 100%;
  height: auto;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
</style>