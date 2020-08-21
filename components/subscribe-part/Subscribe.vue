<template>
  <div class="wrapper">
    <Subtxt />
    <Subinput />
  </div>
</template>

<script>
import Subtxt from "./Subtxt";
import Subinput from "./Subinput";
export default {
  name: "Subscribe",
  components: {
    Subtxt,
    Subinput
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  margin-top: 100px;
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
  @media only screen and (max-width: 1000px) {
    flex-wrap: wrap;
    margin-top: 30px;
  }
}
</style>