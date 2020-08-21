<template>
  <div class="wrapper">
    <h4>Get access to exclusive deals, and the first look at new experiences</h4>
  </div>
</template>

<script>
export default {
  name: "Subtxt"
};
</script>

<style lang="scss" scoped>
.wrapper {
  width: 50%;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  @media only screen and (max-width: 1000px) {
    order: -1;
    justify-content: center;
  }
  @media only screen and (max-width: 768px) {
    width: 100%;
    justify-content: center;
  }

  h4 {
    max-width: 60%;
    line-height: 1.4;
    font-weight: 700;
    font-size: 1.9rem;
    line-height: 2.4rem;
    font-style: normal;
    @media only screen and (max-width: 768px) {
      max-width: 80%;
      text-align: center;
    }
  }
}
</style>