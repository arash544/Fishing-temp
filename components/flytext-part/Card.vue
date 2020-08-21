<template>
  <div class="card">
    <div class="header">
      <img :src="img" alt="alternativ" />
    </div>
    <div class="body">
      <h4>{{header}}</h4>
      <p>{{text}}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Card",
  props: ["img", "header", "text"]
};
</script>

<style lang="scss" scoped>

  .card {
    padding: 10px;
    width: 20%;
    height: auto;
    flex-direction: column;
    display: flex;
    margin-left: 10px;
    border: none;
    @media only screen and (max-width: 768px) {
      width: 95%;
      padding: 0 0 0 10px;
      flex-direction: row;
      margin-left: 0px;
      margin-top: 10px;
    }
  }
  .body {
    @media only screen and (max-width: 768px) {
      margin-left: 20px;
    }
  }
  .header,
  .body {
    margin-top: 20px;
    align-items: center;
    padding-left: 0px;
  }
  p {
    color: gray;
    line-height: 1.3;
    align-items: center;
  }
  h4 {
    font-size: 22px;
    font-weight: 700;
  }
  .header {
    @media only screen and (max-width: 768px) {
      display: flex;
      align-items: center;
    }
  }
  img {
    width: 5vw;
    @media only screen and (max-width: 768px) {
      width: 12vw;
    }
    @media only screen and (max-width: 420px) {
      width: 16vw;
    }
  }

</style>