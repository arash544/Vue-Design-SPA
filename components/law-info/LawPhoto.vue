<template>
  <div class="img-parent">
      <img src="city.jpg" alt="">
  </div>
</template>

<script>
export default {
name:'LawPhoto'
}
</script>

<style lang="scss" scoped>
.img-parent {
  width: 60%;
}
img {
  width: 35vw;
  height: 22vw;
  @media only screen and (max-width: 768px) {
  width: 100vw;
  height: 60vw;
  }
}
</style>