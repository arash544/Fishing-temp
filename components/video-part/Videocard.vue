<template>
  <div class="card">
    <div class="head" :style="bgImg">
      <div class="footer-up">
        <span :style="{ color: color }">{{ position }}</span>
        <span>|</span>
        <h6>{{ country }}</h6>
      </div>
      <div class="footer-down">
        <h4>{{ name }}</h4>
      </div>
      <div class="footer-right">
        <a href="https://www.youtube.com/watch?v=tvDH4JM_gME">
          <img :src="play" alt />
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Videocard",
  props: ["position", "country", "name", "play", "color", "img"],
  computed: {
    bgImg() {
      return `background:linear-gradient(rgba(7, 7, 7, 0.8),rgba(94, 92, 92, 0.8)),url(${this.img}) center center/cover no-repeat`;
    }
  }
};
</script>

<style lang="scss" scoped>
.card {
  width: 20%;
  height: 20%;
  margin-left: 10px;
  border-radius: 0;
  @media only screen and (max-width: 1100px) {
    width: 70%;
    margin-left: 0;
    height: auto;
    margin-top: 20px;
  }
  @media only screen and (max-width: 768px) {
    width: 100%;
  }
}
.head {
  padding-top: 350px;
  width: 100%;
  height: 60vh;
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  position: relative;
  @media only screen and (min-width: 1650px) {
    padding-top: 500px;
  }
  @media only screen and (max-width: 768px) {
    width: 100%;
  }
}

.footer-up {
  display: flex;
  flex-direction: row;
  width: 55%;
  color: #fff;
  align-items: center;
  margin-left: 10px;

  @media only screen and (max-width: 768px) {
    margin-top: -50px;
  }
  @media only screen and (max-width: 330px) {
    margin-top: -100px;
    width: 75%;
  }
}
.footer-down {
  display: flex;
  flex-direction: row;
  width: 60%;
  align-items: center;
  color: #fff;
  @media only screen and (max-width: 330px) {
    width: 75%;
  }
}
.footer-right {
  display: flex;
  flex-direction: row;
  width: 100%;
  justify-content: flex-end;
  margin-top: -55px;
  color: #fff;
}
h4 {
  color: #fff;
}
h6 {
  padding-top: 7px;
}
span,
h6 {
  margin-left: 10px;
}
h4 {
  margin-left: 20px;
}
img {
  margin-right: 25px;
}
</style>
