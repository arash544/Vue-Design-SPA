<template>
  <div class="btn-wrap">
      <button>CONTACT US</button>
  </div>
</template>

<script>
export default {
name:'TopBtn'
}
</script>

<style lang="scss" scoped>
.btn-wrap{
margin-top: 50px;
  display: flex;
  flex-direction: row;
  justify-content: center;
   @media only screen and (max-width: 768px) {
    margin-top: 10px;
    margin-bottom: 10px;
  }

}
button {
  padding: 15px 30px;
  cursor: pointer;
  font-size: 12px;
  outline: none;
  border: 1px solid rgb(7, 7, 7);
  color: white;
  background-color: black;
  text-align: center;
  &:hover {
    outline: none;
    color: black;
    background-color: white;
  }
}
</style>