<template>
  <div class="wrapper">
    <div class="txt-box">
      <div class="title">
        <h1>We travel.</h1>
        <h1>We fish.</h1>
      </div>
      <div class="content">
        <p>Search, discover and book over 1000 fishing experiences, tours, lodges, guides, fisheries and more.</p>
      </div>

      <div class="footer">
        <div class="form-header">
          <img src="location.svg" alt />
          <input
            type="text"
            placeholder="Destination"
            class="dropdown-toggle location-input"
            data-toggle="dropdown"
            aria-haspopup="true"
            aria-expanded="false"
          />
          <div class="dropdown-menu">
            <a class="dropdown-item" href="#">Denmark</a>
            <a class="dropdown-item" href="#">Finland</a>
            <a class="dropdown-item" href="#">Northern Ireland</a>
            <a class="dropdown-item" href="#">Norway</a>
            <a class="dropdown-item" href="#">Sweden</a>
          </div>
        </div>

        <div class="form-body">
          <div class="date">
            <img src="calendar.svg" alt />
            <input
              type="text"
              placeholder="Dates"
              class="dropdown-toggle date-input"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            />
            <div class="dropdown-menu drop">
              <a class="dropdown-item" href="#">12 July</a>
              <a class="dropdown-item" href="#">30 August</a>
              <a class="dropdown-item" href="#">01 September</a>
              <a class="dropdown-item" href="#">18 February</a>
              <a class="dropdown-item" href="#">22 June</a>
              <a class="dropdown-item" href="#">28 May</a>
              <a class="dropdown-item" href="#">10 October</a>
            </div>
          </div>
          <div class="guest">
            <img src="user.svg" alt />
            <input
              type="text"
              placeholder="Guests"
              class="dropdown-toggle guest-input"
              data-toggle="dropdown"
              aria-haspopup="true"
              aria-expanded="false"
            />
            <div class="dropdown-menu drops">
              <a class="dropdown-item" href="#">1</a>
              <a class="dropdown-item" href="#">2</a>
              <a class="dropdown-item" href="#">3</a>
              <a class="dropdown-item" href="#">4</a>
              <a class="dropdown-item" href="#">5</a>
              <a class="dropdown-item" href="#">6</a>
              <a class="dropdown-item" href="#">7</a>
            </div>
          </div>
          <button>Plan my trip</button>
        </div>
      </div>
    </div>
    <Headerimage
      show="true"
      link="Fishing in the wild Alagnak River"
      txt="Hosted-by Planet Fly Fishing in United States of America"
      img="cover.jpeg"
    />
  </div>
</template>

<script>
import Headerimage from "./Headerimage";
export default {
  name: "Headertext",
  components: {
    Headerimage
  }
};
</script>

<style lang="scss" scoped>

.wrapper {
  width: 100%;
  display: flex;
  align-items: center;
  flex-wrap: wrap;
}
.txt-box {
  width: 45%;
  display: flex;
  flex-direction: column;
  padding: 30px;
  align-items: center;
  @media only screen and (max-width: 1000px) {
    width: 100%;
  }

  h1 {
    font-weight: 700;
  }
  p {
    font-weight: 700;
    color: gray;
    line-height: 1.4;
    font-size: 18px;
    max-width: 75%;
    @media only screen and (max-width: 1000px) {
      max-width: 100%;
    }
  }
  .content {
    margin-top: 20px;
  }
  .footer {
    margin-top: 25px;
    width: 100%;
  }
  .form-header {
    display: flex;
    input {
      padding: 30px;
      border: none;
      width: 100%;
    }
    img {
      padding: 10px;
    }
  }
  .title,
  .content,
  .footer {
    width: 80%;
  }
  .form-body {
    width: 100%;
    display: flex;
    flex-direction: row;
    align-items: center;
    input {
      width: 100%;
      border: none;
    }
    img {
      padding: 10px;
    }
  }
  .date,
  .guest {
    display: flex;
    height: 100px;
    flex-direction: row;
    @media only screen and (max-width: 1000px) {
      display: none;
    }
  }

  button {
    background-color: #56d2ab;
    font-size: 14px;
    font-weight: 700;
    color: white;
    width: 30%;
    border: none;
    // padding-top: 35px;
    // padding-bottom: 35px;
    height: 100px;
    @media only screen and (max-width: 1000px) {
      // padding-top: 30px;
      // padding-bottom: 30px;
      width: 100%;
    }
  }

  .dropdown-menu {
    width: 30%;
    line-height: 1.7;
  }
  .drop {
    width: 5%;
    line-height: 1.7;
  }
  .drops {
    width: 5%;
    line-height: 1.7;
  }
  input {
    outline: none;
  }
}
</style>