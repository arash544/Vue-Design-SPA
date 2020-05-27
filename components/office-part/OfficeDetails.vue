<template>
  <div class="office-parent">
    <div class="wrapper">
      <div class="txt-part">
        <h1>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Doloribus, deserunt!</h1>
        <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Deserunt quasi quod commodi nam temporibus ratione exercitationem voluptas saepe animi sapiente.</p>
        <button>CONTACT US</button>
      </div>
      <OfficePhoto />
    </div>
  </div>
</template>

<script>
import OfficePhoto from "./OfficePhoto";
export default {
  name: "OfficeDetails",
  components: {
    OfficePhoto
  }
};
</script>

<style lang="scss" scoped>
.office-parent {
  height: 900px;
  width: 45%;
  border: 1px solid lightgray;
  display: flex;
  flex-direction: row;
  box-shadow: 0 10px 20px -6px rgba(114, 113, 113, 0.623);
  @media only screen and (max-width: 768px) {
    width: 100vw;
    flex-direction: column;
    margin-top: -30px;
    min-height: 900px;
  }
}
.wrapper {
  width: 100%;
  display: flex;
  flex-direction: row;
  @media only screen and (max-width: 768px) {
    width: 100vw;
    flex-direction: column;
    margin-top: 20px;
  }
}
.txt-part {
  width: 40%;
  padding-top: 150px;
  @media only screen and (max-width: 768px) {
    width: 100vw;
    padding-top: 20px;
    text-align: center;
    padding-left: 20px;
    padding-right: 20px;
  }
}
button {
  padding: 15px 30px;
  outline: none;
  cursor: pointer;
  font-size: 12px;
  outline: none;
  border: 1px solid rgb(7, 7, 7);
  color: white;
  background-color: black;
  &:hover {
    outline: none;
    color: black;
    background-color: white;
  }
}
h1,
p,
button {
  margin-left: 10px;
}
h1 {
  font-size: 28px;
}
p {
  margin-top: 10px;
  color: gray;
}
button {
  margin-top: 20px;
}
</style>