<template>
  <div class="wrapper">
    <div class="head">
      <img :src="img" alt />
    </div>
    <div class="body">
      <p>{{txt}}</p>
      <h6>
        {{starttext}}
        <a href="/">{{link}}</a>
        {{endtext}}
      </h6>
    </div>
  </div>
</template>

<script>
export default {
  name: "Gueststxt",
  props: ["img", "txt", "starttext", "endtext", "link"]
};
</script>

<style lang="scss" scoped>
.wrapper {
  display: flex;
  flex-direction: column;
  padding: 0px;
  align-items: center;
  flex-wrap: wrap;
  justify-content: center;
  @media only screen and (max-width: 1000px) {
    padding: 20px;
    width: 100%;
    margin-bottom: 100px;
  }
}
.head {
  display: flex;
  width: 30%;
  align-items: center;
  justify-content: flex-start;
  flex-direction: row;
  @media only screen and (max-width: 1000px) {
    width: 100%;
    justify-content: flex-start;
  }
  img {
    align-items: center;
    justify-content: center;
  }
}
.body {
  display: flex;
  justify-content: flex-end;
  align-items: flex-end;
  width: 50%;
  flex-direction: column;
  @media only screen and (max-width: 1000px) {
    align-items: flex-start;
    justify-content: flex-start;
    width: 100%;
  }
  p {
    width: 70%;
    font-size: 0.9rem;
    line-height: 1.4rem;
    font-weight: 400;
    color: rgb(73, 72, 72);
    @media only screen and (max-width: 1000px) {
      width: 100%;
    }
  }
  h6 {
    width: 70%;
    font-weight: 600;
    font-size: 16px;
    @media only screen and (max-width: 1000px) {
      width: 100%;
    }
  }
  a {
    color: black;
    text-decoration: underline;
  }
}
</style>