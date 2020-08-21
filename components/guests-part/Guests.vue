<template>
  <div class="wrapper" :style="styles">
    <Gueststxt
      img="quote.svg"
      txt="Fly-Fishing in Argentina was one of the best experiences I’ve ever had (and I’ve had a lot..). Stunning scenery together with a wide choice of fishing spots makes Patagonia one of the most promising fly-fishing destination ever!"
      starttext="With"
      link="Spring Creek Lodge"
      endtext="- Argentina"
    />
    <Headerimage class="photo" size="32%" img="fisher.jpg" />
  </div>
</template>

<script>
import Headerimage from "@/components/header-part/Headerimage";
import Gueststxt from "./Gueststxt";
export default {
  name: "Guests",
  components: {
    Headerimage,
    Gueststxt
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  margin-top: 50px;
  width: 100%;
  display: flex;
  align-items: center;

  @media only screen and (max-width: 1000px) {
    flex-wrap: wrap;
  }
}
.photo {
  margin-right: 60px;
  @media only screen and (max-width: 1000px) {
    margin-right: 0;
  }
}
</style>