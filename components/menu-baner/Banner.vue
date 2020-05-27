<template>
  <div class="baner-parent">
    <div class="overlay">
      <Navbar />
      <Details />
    </div>
  </div>
</template>

<script>
import Navbar from "./Navbar";
import Details from "./Details";
export default {
  name: "Banner",
  components: {
    Navbar,
    Details
  }
};
</script>

<style lang="scss" scoped>
.baner-parent {
  background: url("https://i.picsum.photos/id/214/2729/2047.jpg")
    no-repeat center;
  background-size: cover;
  position: relative;
  height: 1000px;
  width: 45%;
  border: 1px solid lightgray;
  box-shadow:0 10px 20px -6px rgba(114, 113, 113, 0.623);
   @media only screen and (max-width: 768px) {
       width:100vw;
   }
}
.overlay {
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
}
</style>