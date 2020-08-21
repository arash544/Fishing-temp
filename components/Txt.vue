<template>
  <div class="wrapp">
    <h2>{{head}}</h2>
    <p v-if="show">{{desc}}</p>
  </div>
</template>

<script>
export default {
  name: "Txt",
  props: ["head", "desc", "show"]
};
</script>

<style lang="scss" scoped>

.wrapp {
  width: 80%;
  margin-top: 150px;
  display: flex;
  flex-direction: column;
  align-items: center;
  @media only screen and (max-width: 768px) {
    width: 100%;
    text-align: center;
    padding: 15px;
    margin-left: 0;
  }
  h2 {
    font-weight: 700;
    font-size: 1.9rem;
    line-height: 2.4rem;
    font-style: normal;
    width: 50%;
    @media only screen and (max-width: 768px) {
      width: 100%;
    }
  }
  p {
    max-width: 50%;
    margin-top: 0.6rem;
    font-size: 100%;
    font-style: normal;
    line-height: 1.4rem;
    color: rgb(105, 103, 103);
    @media only screen and (max-width: 768px) {
      max-width: 100%;
    }
  }
}
</style>