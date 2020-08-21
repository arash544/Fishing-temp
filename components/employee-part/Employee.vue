<template>
  <div class="wrapper">
    <Employeecard
      img="fisher-1.png"
      header="Quentin W."
      text="Brussels, Belgium"
    />
    <Employeecard
      img="girl.jpg"
      header="Nicholas B."
      text="Vienna, Austria"
    />
    <Employeecard
      img="fisher-3.png"
      header="Baudoin T."
      text="Berlin, Germany"
    />
  </div>
</template>

<script>
import Employeecard from "./Employeecard";
export default {
  name: "Employee",
  components: {
    Employeecard
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin-top: 100px;
  flex-wrap: wrap;
  @media only screen and (max-width: 768px) {
    margin-top: 50px;
  }
}
</style>