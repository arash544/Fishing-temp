<template>
  <div class="wrap">
    <div class="banner">
      <Textbanner />
    </div>
  </div>
</template>

<script>
import Textbanner from "./Textbanner";
export default {
  name: "Imagebanner",
  components: {
    Textbanner
  }
};
</script>

<style lang="scss" scoped>
.banner {
  width: 60%;
  height: 60vh;
  background-image: linear-gradient(rgba(7, 7, 7, 0.8), rgba(94, 92, 92, 0.8)),
    url(/girl.jpg);
  background-size: cover;
  background-position: top;
  position: relative;
  @media only screen and (max-width: 768px) {
    width: 100%;
  }
}

.wrap {
  margin-top: 120px;
  display: flex;
  justify-content: center;
}
</style>