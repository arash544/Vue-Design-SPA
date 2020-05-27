<template>
  <div class="text-parent">
    <h1>Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi unde dolor quo vitae.</h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Hic laudantium doloribus tempore inventore adipisci? Eius soluta facere labore doloribus inventore? Nisi odio aut doloribus vero? Quos excepturi debitis ipsum. Omnis, ducimus asperiores numquam ut possimus sint impedit debitis, aliquam maxime iste veniam hic nisi eius quisquam sequi dolor perspiciatis quia cumque eveniet laborum quam repellendus dolorum repudiandae! Recusandae labore quo voluptas, optio error ea. Exercitationem dicta totam libero laudantium porro?</p>
    <div class="btn-parent">
      <button class="btn-txt-cu">CONTACT US</button>
      <button class="btn-txt-pa">PRACTICE AREAS</button>
    </div>
  </div>
</template>

<script>
export default {
  name: "Details"
};
</script>

<style lang="scss" scoped>
.text-parent {
  margin-top: 50px;
  color: white;
  margin-left: 15px;
  @media only screen and (max-width: 768px) {
    text-align: center;
  }
}
h1 {
  font-size: 45px;
  @media only screen and (max-width: 768px) {
    text-align: center;
  }
}
p {
  margin-top: 20px;
  @media only screen and (max-width: 768px) {
    text-align: center;
  }
}
.btn-parent {
  margin-top: 40px;
}
.btn-txt-cu {
  padding: 15px 20px;
  outline: none;
  cursor: pointer;
  font-size: 10px;
  outline: none;
  border: 1px solid white;
}
.btn-txt-pa {
  background-color: transparent;
  color: white;
  border: 1px solid white;
  padding: 15px 20px;
  cursor: pointer;
  font-size: 10px;
  outline: none;
  margin-left: 10px;
}
</style>