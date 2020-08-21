<template>
  <nav>
    <ul class="logo-parent" ref="menu">
      <li>
        <a href="/">
          <img  src="fish.png" alt />
        </a>
      </li>
    </ul>
    <ul class="link-parent" ref="menu">
      <li class="img-collapse">
        <img class="logo" src="fish.png" alt />
      </li>
      <li>
        <a href="/">Fishing</a>
      </li>
      <li>
        <a href="/">Hosting</a>
      </li>
      <li>
        <a href="/">Scouting</a>
      </li>
      <li>
        <a href="/">About</a>
      </li>
      <li>
        <a href="/">
          <svg
            data-v-d9c07b90
            data-v-762647cf
            xmlns="http://www.w3.org/2000/svg"
            width="21"
            height="21"
            viewBox="0 0 21 21"
          >
            <path
              data-v-d9c07b90
              data-v-762647cf
              fill="#353745"
              stroke="#353745"
              stroke-width=".5"
              d="M17.2235772,4.63414634 L13.3,4.63414634 C13.9487805,4.18617886 14.3658537,3.44471545 14.3658537,2.59512195 C14.3658537,1.15853659 13.2227642,0 11.8170732,0 C10.7821138,0 9.90162602,0.617886179 9.5,1.51382114 C9.09837398,0.617886179 8.21788618,0 7.18292683,0 C5.77723577,0 4.63414634,1.15853659 4.63414634,2.59512195 C4.63414634,3.44471545 5.05121951,4.18617886 5.7,4.63414634 L1.77642276,4.63414634 C0.803252033,4.63414634 0,5.43739837 0,6.41056911 L0,9.5 C0,9.62357724 0.108130081,9.73170732 0.231707317,9.73170732 L0.926829268,9.73170732 L0.926829268,17.2235772 C0.926829268,18.196748 1.7300813,19 2.70325203,19 L16.296748,19 C17.2699187,19 18.0731707,18.196748 18.0731707,17.2235772 L18.0731707,9.73170732 L18.7682927,9.73170732 C18.8918699,9.73170732 19,9.62357724 19,9.5 L19,6.41056911 C19,5.43739837 18.196748,4.63414634 17.2235772,4.63414634 Z M11.8170732,0.463414634 C12.9601626,0.463414634 13.902439,1.42113821 13.902439,2.59512195 C13.902439,3.73821138 12.9910569,4.63414634 11.8170732,4.63414634 L9.73170732,4.63414634 L9.73170732,2.59512195 C9.73170732,1.42113821 10.6739837,0.463414634 11.8170732,0.463414634 Z M5.09756098,2.59512195 C5.09756098,1.42113821 6.0398374,0.463414634 7.18292683,0.463414634 C8.32601626,0.463414634 9.26829268,1.42113821 9.26829268,2.59512195 L9.26829268,4.63414634 L7.18292683,4.63414634 C6.00894309,4.63414634 5.09756098,3.73821138 5.09756098,2.59512195 Z M17.6097561,17.2235772 C17.6097561,17.9495935 17.0227642,18.5365854 16.296748,18.5365854 L2.70325203,18.5365854 C1.97723577,18.5365854 1.3902439,17.9495935 1.3902439,17.2235772 L1.3902439,9.73170732 L17.6097561,9.73170732 L17.6097561,17.2235772 Z M18.5365854,9.26829268 L0.463414634,9.26829268 L0.463414634,6.41056911 C0.463414634,5.68455285 1.0504065,5.09756098 1.77642276,5.09756098 L7.18292683,5.09756098 L9.5,5.09756098 L11.8170732,5.09756098 L17.2235772,5.09756098 C17.9495935,5.09756098 18.5365854,5.68455285 18.5365854,6.41056911 L18.5365854,9.26829268 Z"
              transform="translate(1 1)"
            />
          </svg> Gift Cards
        </a>
      </li>
      <li>
        <a href="/">
          Refer a friend
          <button class="btn-new">New</button>
        </a>
      </li>
      <li class="btn-collapse">
        <button>See all experiences</button>
      </li>
    </ul>
    <ul class="login-parent">
      <button @click="showMenu" class="menu-icon">
        <svg
          height="25"
          width="25"
          data-v-d9c07b90
          xmlns="http://www.w3.org/2000/svg"
          viewBox="0 0 24 18"
          class="icon-burger-nav"
        >
          <g
            data-v-d9c07b90
            fill="none"
            fill-rule="evenodd"
            stroke="#353745"
            stroke-linecap="square"
            stroke-width="1.5"
            transform="translate(0)"
          >
            <path data-v-d9c07b90 d="M0 1L18 1M0 9L13 9M0 17L22 17" />
          </g>
        </svg>
      </button>
      <li>
        <a href="/">Log in</a>
      </li>
      <li>
        <a href="/" class="btn-hosting">Start hosting</a>
      </li>
    </ul>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
  methods: {
    showMenu() {
      this.$refs["menu"].classList.toggle("menu-block");
    }
  }
};
</script>

<style lang="scss" scoped>

.img-collapse {
  display: none;
  @media only screen and (max-width: 1100px) {
    display: block;
    margin-bottom: 50px;
    img {
      width: 100px;
    }
  }
}
.btn-collapse {
  display: none;
  @media only screen and (max-width: 1100px) {
    display: block;
    display: flex;
    width: 100%;
    button {
      background-color: #56d2ab;
      color: white;
      padding: 10px 150px;
      border: none;
      margin-top: 700px;
      font-weight: 700;
      @media only screen and (max-width: 550px) {
        padding: 10px 30px;
        margin-left: -150px;
      }
    }
  }
}
.menu-icon {
  background-color: transparent;
  border-radius: 10px;
  font-size: 14px;
  outline: none;
  border: none;
  margin-top: -5px;
  cursor: pointer;
  display: none;
  outline: none;
  @media only screen and (max-width: 1100px) {
    display: block;
    z-index: 1000;
    position: relative;
    outline: none;
    &:active,
    &:hover,
    &:focus {
      outline: none;
    }
  }
}
li {
  list-style-type: none;
  @media only screen and (max-width: 1100px) {
    margin-top: 5px;
  }
}
nav {
  width: 100%;
  left: 0;
  right: 0;
  top: 0;
  position: fixed;
  display: flex;
  align-items: center;
  justify-content: space-between;
  flex-wrap: wrap;
  font-weight: 300;
  font-size: 15px;
  background-color: #fff;
  z-index: 2000;
}
.logo-parent {
  width: 15%;
  justify-content: flex-start;
  @media only screen and (max-width: 1100px) {
    order: -1;
  }
  img {
     width: 100px;
    @media only screen and (max-width: 768px) {
      // width: 35vw;
    }
  }
}
.hide-btn {
  display: none;
  @media only screen and (max-width: 480px) {
    display: block;
  }
}
.logo-parent,
.login-parent,
.link-parent {
  display: flex;
  flex-direction: row;
  align-items: center;
  flex-wrap: wrap;
  margin-top: 10px;
}
.link-parent {
  width: 50%;
  justify-content: space-evenly;
  a {
    color: black;
    text-decoration: none;
  }
  .btn-new {
    background-color: red;
    color: white;
    border: none;
  }
  @media only screen and (max-width: 1100px) {
    position: absolute;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: baseline;
    top: -10px;
    bottom: 0;
    left: -100%;
    right: 0;
    width: 100%;
    height: 100vh;
    line-height: 2;
    padding: 20px;
    transition: all 2s ease-in-out;
    background-color: #fff;
    cursor: pointer;

    &.menu-block {
      left: 0px;
    }
  }
}

.login-parent {
  width: 30%;
  justify-content: flex-end;
  padding-right: 10px;
  a {
    color: black;
    text-decoration: none;
    padding-right: 10px;
    &.btn-hosting {
      margin-right: 20px;
      padding: 15px 22px;
      border: 1px solid black;
      border-radius: 5px;
      font-weight: 700;
      font-size: 14px;
      @media only screen and (max-width: 1000px) {
        display: none;
      }
    }
  }
  @media only screen and (max-width: 900px) {
    width: 60%;
  }
}
.logo {
  width: 10px;
  // @media only screen and (max-width: 700px) {
  //   width:10px
  // }
}
</style>