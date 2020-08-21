<template>
  <div class="card">
    <div class="head">
      <h6>{{head}}</h6>
      <h3>{{title}}</h3>
    </div>
    <div class="body">
      <p>{{txt}}</p>
    </div>
    <div class="footer">
      <a href="/">{{link}}</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Textbanner",
  props: ["head", "title", "txt", "link"]
};
</script>

<style lang="scss" scoped>
.card,
a {
  color: #fff;
}
.card {
  margin-top: 0px;
  background-color: transparent;
  height: 100%;
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  position: absolute;
  z-index: 1100;
  border: none;
}
.head,
.body,
.footer {
  padding-left: 350px;
  @media only screen and (max-width: 768px) {
    padding-left: 15px;
    padding-right: 15px;
  }
  @media only screen and (min-width: 1650px) {
    padding-left: 450px;
  }
  @media only screen and (min-width: 1024px) {
    padding-left: 250px;
  }
}
.head {
  display: flex;
  flex-direction: column;
  h3 {
    width: 50%;
    @media only screen and (max-width: 768px) {
      width: 100%;
    }
  }
  h6,
  h3 {
    font-weight: 900;
  }
}
.body {
  display: flex;
  flex-direction: column;
  p {
    width: 30%;
    line-height: 1.4;
    font-weight: 300;
    @media only screen and (max-width: 768px) {
      width: 100%;
    }
  }
}
</style>