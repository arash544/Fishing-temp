<template>
  <div class="card">
    <img :src="img" alt />
    <h5>{{header}}</h5>
    <h6>{{text}}</h6>
  </div>
</template>

<script>
export default {
  name: "Employeecard",
  props: ["img", "header", "text"]
};
</script>

<style lang="scss" scoped>
.card {
  width: 25%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  border: none;
  align-items: center;
  @media only screen and (max-width: 768px) {
    width: 100%;
  }
  img {
    width: 80px;
    height: 80px;
    object-fit: cover;
    border-radius: 100%;
    margin-top: 10px;
    margin-bottom: 10px;
    @media only screen and (max-width: 768px) {
      width: 50px;
      height:50px
    }
  }
  h5 {
    font-size: 14px;
    font-weight: 600;
  }
  h6 {
    font-size: 16px;
    font-weight: 600;
    color: rgb(138, 132, 132);
  }
}
</style>