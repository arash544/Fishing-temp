<template>
  <div class="wrappers">
    <img :src="img" alt width="90%" />
    <div class="txt" v-if="show">
      <a href="/">{{link}}</a>
      <h6>{{txt}}</h6>
    </div>
  </div>
</template>

<script>
export default {
  name: "Headerimage",
  props: {
    img: String,
    link: String,
    txt: String,
    show: String,
    size: {
      type: String,
      default: "42%"
    }
  }
};
</script>

<style lang="scss" scoped>
.wrappers {
  display: flex;
  width: 55%;
  align-items: center;
  flex-direction: column;
  @media only screen and (max-width: 1000px) {
    margin-top: -80px;
    width: 100%;
    position: relative;
    z-index: -100;
    align-items: center;
  }
  .txt {
    margin-top: 5px;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: flex-end;
    width: 90%;
    @media only screen and (max-width: 1000px) {
      display: none;
    }
  }
  img {
    @media only screen and (max-width: 1000px) {
      width: 100%;
    }
  }

  a {
    color: black;
    text-decoration: underline;
    font-weight: 600;
  }

  a,
  h6 {
    font-size: 12px;
    margin-left: 10px;
  }
  h6 {
    color: gray;
    margin-top: 10px;
  }
}
</style>