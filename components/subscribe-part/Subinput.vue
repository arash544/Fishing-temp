<template>
  <div class="wrapper">
    <input type="text" placeholder="Enter your best email ;)" />
    <button>Subscribe</button>
  </div>
</template>

<script>
export default {
  name: "Subinput"
};
</script>

<style lang="scss" scoped>
.wrapper {
  width: 50%;
  display: flex;
  justify-content: center;
  align-items: center;

  @media only screen and (max-width: 768px) {
    width: 100%;
  }

  input {
    height: 100px;
    width: 45%;
    padding-left: 15px;
    border: 1px solid lightgray;
    font-weight: 400;
    font-size: 20px;
    border-bottom-left-radius: 5px;
    border-top-left-radius: 5px;

    @media only screen and (max-width: 768px) {
      width: 80%;
      border-radius: unset;
      height: 80px;
    }
  }
  button {
    background-color: #56d2ab;
    font-size: 14px;
    font-weight: 700;
    color: white;
    width: 15%;
    border: 1px solid #56d2ab;
    height: 100px;
    @media only screen and (max-width: 768px) {
      width: 80%;
      height: 60px;
    }
  }
}
</style>