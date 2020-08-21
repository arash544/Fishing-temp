<template>
  <div class="wrapper">
    <Card
      img="fish.svg"
      header="Search and compare"
      text="hundreds of fishing experiences around the world handpicked by Fishtripr."
    />
    <Card
      img="compass.svg"
      header="Plan your trip"
      text="with our fishing advisor and customize a unique fishing trip to your needs."
    />
    <Card
      img="boat.svg"
      header="Book and travel"
      text="safely with Fishtripr through our secure payment system and guarantee satisfaction."
    />
  </div>
</template>

<script>
import Card from "./Card";
export default {
  name: "Flytxt",
  components: {
    Card
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  margin-top: 120px;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
}
</style>