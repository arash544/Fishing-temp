<template>
  <div class="wrapper">
    <Videocard
      img="fisher-1.png"
      color="#36befb"
      position="Hosting"
      country="Bolivia"
      name="Emilio e Giorgio"
      play="play.svg"
    />
    <Videocard
      img="fisher-2.png"
      color="#be7a0b"
      position="Guide"
      country="Denmark"
      name="Bjarke Borup"
      play="play.svg"
    />
    <Videocard
      img="fisher-3.png"
      color="pink"
      position="Guide, Hosting"
      country="Bolivia"
      name="Marcelo Pérez"
      play="play.svg"
    />
  </div>
</template>

<script>
import Videocard from "./Videocard";
export default {
  name: "Video",
  components: {
    Videocard
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  margin-top: 120px;
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
  flex-wrap: wrap;
  @media only screen and (max-width: 1100px) {
    flex-direction: column;
  }
}
</style>