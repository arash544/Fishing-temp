<template>
  <div class="wrapper">
    <div class="top-footer">
      <div class="col-txt">
        <h4>Fishtripr is everywhere you want to go</h4>
        <p>Discover unique fishing experiences on ranches, nature preserves, farms, vineyards, and public campgrounds access the world. Book guides, lodges, charters and boats, fisheries, immersive experiences with guides and hosting, and more...</p>
      </div>
      <div class="col-browse">
        <h4>Browse</h4>
        <a href="/">Explore trips</a>
        <a href="/">Plan</a>
        <a href="/">Help</a>
        <a href="/">Contact</a>
        <a href="/">Gift Cards</a>
      </div>
      <div class="col-about">
        <h4>About</h4>
        <a href="/">Blog</a>
        <a href="/">Our story</a>
        <a href="/">Press Kit</a>
      </div>
      <div class="col-social">
        <h4>Social</h4>
        <div class="fb">
          <img src="facebook.png" alt />
          <a class="link" href="/">Facebook</a>
        </div>
        <div class="insta">
          <img src="instagram.png" alt />
          <a class="link" href="/">Instagram</a>
        </div>
        <div class="linkedin">
          <img src="linkedin.png" alt />
          <a class="link" href="/">Linkedin</a>
        </div>
        <div class="twitter">
          <img src="twitter.png" alt />
          <a class="link" href="/">Twitter</a>
        </div>
      </div>
    </div>
    <div class="hr">
      <hr />
    </div>
    <div class="footer">
      <h6>© 2020 Fishtripr. All rights reserved.</h6>
      <h6>
        <a href="/">Terms of services</a>
        <span>-</span>
        <a href="/">Privacy policy</a>
      </h6>
    </div>
  </div>
</template>

<script>
export default {
  name: "Footer"
};
</script>

<style lang="scss" scoped>
.top-footer {
  width: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-evenly;
  flex-wrap: wrap;
  padding-top: 100px;
  @media only screen and (max-width: 768px) {
    flex-direction: column;
  }
}
.wrapper {
  margin-top: 120px;
  background-color: #353745;
  width: 100%;
  height: auto;
  align-items: center;
  justify-content: center;
  color: white;
  .col-txt {
    width: 30%;
    height: 300px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    justify-content: flex-start;
    @media only screen and (max-width: 768px) {
      width: 100%;
      height: auto;
      align-items: center;
    }
  }
  a,
  h4,
  img {
    margin-top: 5px;
        @media only screen and (max-width: 768px) {
      margin-top: 0px;
    }
  }
  .link {
    margin-left: 7px;
    @media only screen and (max-width: 768px) {
      margin-left: 0px;
    }
  }

  a,
  p,
  h6 {
    color: white;
    font-size: 12px;
  }
  a {
    @media only screen and (max-width: 768px) {
      margin-left: 5px;
    }
  }
  p {
    max-width: 100%;
    line-height: 1.4;
    @media only screen and (max-width: 768px) {
      max-width: 60%;
    }
  }
  h4 {
    max-width: 100%;
    font-size: 16px;
    font-weight: 700;
    @media only screen and (max-width: 768px) {
      max-width: 60%;
      padding-top: 10px;
    }
  }
  .col-browse,
  .col-about,
  .col-social {
    display: flex;
    flex-direction: column;
    width: 15%;
    padding: 10px;
    align-self: flex-start;
    // border: 1px solid gray;
    @media only screen and (max-width: 768px) {
      width: 100%;
      padding: 2px;
      align-items: center;
      flex-direction: row;
      justify-content: center;
    }
  }
  .hr {
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    justify-content: center;
    background-color: white;
    @media only screen and (max-width: 768px) {
      display: none;
    }
  }
  hr {
    margin-top: -120px;
    background-color: white;
    width: 60%;
    @media only screen and (max-width: 768px) {
      margin-top: 0;
      display: none;
    }
  }
  .footer {
    display: flex;
    justify-content: space-evenly;
    padding-bottom: 30px;
    flex-wrap: wrap;
    @media only screen and (max-width: 768px) {
      margin-top: 10px;
    }
  }
}
.fb,
.insta,
.twitter,
.linkedin {
  @media only screen and (max-width: 768px) {
    margin-left: 5px;
    flex-wrap: wrap;
  }
}
</style>