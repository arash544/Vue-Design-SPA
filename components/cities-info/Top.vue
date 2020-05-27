<template>
  <div class="wrapper">
    <div class="text-parent">
      <h2>Lorem, ipsum.</h2>
      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Nihil atque quia quaerat eveniet at a sed sapiente eaque, voluptas velit. Enim harum nisi rerum iste facilis vel aliquam exercitationem quo!</p>
    </div>
    <TopCity />
    <TopBtn />
  </div>
</template>

<script>
import TopCity from "./TopCity";
import TopBtn from "./TopBtn";
export default {
  name: "Top",
  components: {
    TopCity,
    TopBtn
  }
};
</script>

<style lang="scss" scoped>
.wrapper {
  height: 1000px;
  width: 45%;
  border: 1px solid lightgray;
  box-shadow: 0 10px 20px -6px rgba(114, 113, 113, 0.623);
  @media only screen and (max-width: 768px) {
    width: 100%;
    margin-top: 20px;
    height: auto;
  }
}
.text-parent {
  display: flex;
  flex-direction: column;
  width: 50%;
  padding-left: 20px;
  @media only screen and (max-width: 768px) {
    width: 100%;
    text-align: center;
  }
}
p {
  color: gray;
  padding-top: 10px;
  @media only screen and (max-width: 768px) {
    margin-left: 20px;
    margin-right: 20px;
  }
}
h2 {
  font-size: 32px;
}
</style>