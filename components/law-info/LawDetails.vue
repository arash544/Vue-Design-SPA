<template>
  <div class="banner-parent">
    <div class="wrapper">
      <div class="text-parent">
        <h1>Lorem ipsum dolor sit amet.</h1>
        <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis ducimus error illum? Porrovoluptates doloremque deleniti. Architecto aspernatur reiciendis culpa neque ullam minus. Aspernatur, voluptatum.</p>
        <button>CONTACT US</button>
        <div class="contact">
          <img src="facebook.png" alt />
          <img src="pintrest.png" alt />
          <img src="instagram2.png" alt />
          <img src="soundcloud.png" alt />
          <img src="Twitter.png" alt />
        </div>
      </div>
      <LawPhoto />
    </div>
  </div>
</template>

<script>
import LawPhoto from "./LawPhoto";
export default {
  name: "LawDetails",
  components: {
    LawPhoto
  }
};
</script>

<style lang="scss" scoped>
.banner-parent {
  position: relative;
  color: white;
  height: 900px;
  width: 45%;
  border: 1px solid lightgray;
  background-color: black;
  display: flex;
  flex-direction: column;
  box-shadow: 0 10px 20px -6px rgba(114, 113, 113, 0.623);
  @media only screen and (max-width: 768px) {
    width: 100%;
    margin-top: 20px;
  }
}
.wrapper {
  width: 100%;
  display: flex;
  @media only screen and (max-width: 768px) {
    display: flex;
    flex-direction: column-reverse;
    width: 100%;
  }
}
.text-parent {
  position: absolute;
  bottom: 0;
  right: 0;
  width: 40%;
  padding: 30px 20px;
  @media only screen and (max-width: 768px) {
    width: 100%;
    text-align: center;
    padding-top: 100px;
  }
}
button {
  padding: 15px 30px;
  outline: none;
  cursor: pointer;
  font-size: 12px;
  outline: none;
  border: 1px solid white;
  color: black;
  background-color: white;
  &:hover {
    outline: none;
    color: white;
    background-color: black;
  }
}
h1,
p,
button {
  margin-left: 10px;
}
h1 {
  font-size: 38px;
}
p {
  margin-top: 10px;
}
button {
  margin-top: 20px;
}
.contact {
  display: flex;
  margin-top: 25px;
  padding-bottom: 40px;
  width: 100%;
  padding-left: 10px;
  @media only screen and (max-width: 768px) {
    justify-content: center;
  }
}
img {
  width: 10%;
  // &:hover {
  //   transform: scale(2);
  // }
  @media only screen and (max-width: 768px) {
    width: 7%;
  }
}
</style>