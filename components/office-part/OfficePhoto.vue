<template>
  <div class="img-parent">
    <img src="office.jpg" alt />
  </div>
</template>

<script>
export default {
  name: "OfficePhoto"
};
</script>

<style lang="scss" scoped>
.img-parent {
  width: 60%;
  padding-top: 150px;
  @media only screen and (max-width: 768px) {
    width: 100vw;
    padding-top: 20px;
  }
}
img {
  width: 26.5vw;
  height: 28vw;
  @media only screen and (max-width: 768px) {
  width: 100vw;
  height: 80vw;
  }
}
</style>