<template>
  <nav>
    <button @click="showMenu" class="menu-icon">
      <svg
        id="Layer_1"
        enable-background="new 0 0 512 512"
        height="25"
        viewBox="0 0 512 512"
        width="25"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="m464.883 64.267h-417.766c-25.98 0-47.117 21.136-47.117 47.149 0 25.98 21.137 47.117 47.117 47.117h417.766c25.98 0 47.117-21.137 47.117-47.117 0-26.013-21.137-47.149-47.117-47.149z"
        />
        <path
          d="m464.883 208.867h-417.766c-25.98 0-47.117 21.136-47.117 47.149 0 25.98 21.137 47.117 47.117 47.117h417.766c25.98 0 47.117-21.137 47.117-47.117 0-26.013-21.137-47.149-47.117-47.149z"
        />
        <path
          d="m464.883 353.467h-417.766c-25.98 0-47.117 21.137-47.117 47.149 0 25.98 21.137 47.117 47.117 47.117h417.766c25.98 0 47.117-21.137 47.117-47.117 0-26.012-21.137-47.149-47.117-47.149z"
        />
      </svg>
    </button>
    <ul ref="menu">
      <li>
        <div class="wrap" href="/">
          <img src="pngwing.com.png" alt />
        </div>
      </li>
      <li>
        <a href="/">ABOUT US</a>
      </li>
      <li>
        <a href="/">PRACTICE AREAS</a>
      </li>
      <li>
        <a href="/">CASE RESULTS</a>
      </li>
      <li>
        <button class="nav-btn">CONTACT US</button>
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
.menu-icon {
  background-color: white;
  padding: 2px 10px 0px 10px;
  border-radius: 10px;
  font-size: 14px;
  margin-left: 20px;
  outline: none;
  border: none;
  margin-top: 20px;
  cursor: pointer;
  display: none;
  outline: none;
  @media only screen and (max-width: 768px) {
    display: block;
    z-index: 1000;
    position: relative;
    outline: none;
    &:active,
    &:hover,
    &:focus
    {
      outline: none;
    }
  }
}
.wrap {
  display: block;
}
img {
  width: 3vw;
  margin: -15px auto;
  @media only screen and (max-width: 768px) {
    width: 15vw;
    margin: 0;
  }
}
nav {
  width: 100%;
  border-bottom: 1px solid white;
  height: 80px;
}
ul {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  @media only screen and (max-width: 768px) {
    position: absolute;
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    top: 0px;
    bottom: 0;
    left: 0;
    left: -100%;
    right: 0;
    background-color: black;
    width: 100%;
    color: #fff;
    transition: all 2s ease-in-out;
    cursor: pointer;

    &.menu-block {
      left: 0px;
    }
  }
}
li {
  list-style-type: none;
  margin: 20px auto;
}
a {
  color: white;
  text-decoration: none;
}
.nav-btn {
  padding: 7px 15px;
  border: 1px solid white;
  cursor: pointer;
  outline: none;
  font-size: 10px;
  &:hover {
    background-color: transparent;
    color: white;
    outline: none;
    border: 1px solid white;
  }
}
</style>