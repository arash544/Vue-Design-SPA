<template>
  <div class="wrap">
    <div class="parent">
      <img src="1.jpg" alt />
      <img src="2.jpg" alt />
      <img src="3.jpg" alt />
    </div>
    <div class="txt-parent">
      <div class="txt">
        <div class="side">
          <h3>2341800$</h3>
          <h5>Lorem, ipsum.</h5>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit excepturi eveniet accusantium veniam, aut aliquid sed sint provident reprehenderit.</p>
        </div>
        <div class="back">LONDON</div>
      </div>
      <div class="txt">
        <div class="side">
          <h3>2341800$</h3>
          <h5>Lorem, ipsum.</h5>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit excepturi eveniet accusantium veniam, aut aliquid sed sint provident reprehenderit.</p>
        </div>
        <div class="back">NEW YORK</div>
      </div>
      <div class="txt">
        <div class="side">
          <h3>2341800$</h3>
          <h5>Lorem, ipsum.</h5>
          <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odit excepturi eveniet accusantium veniam, aut aliquid sed sint provident reprehenderit.</p>
        </div>
        <div class="back">TORONTO</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "TopCity"
};
</script>

<style lang="scss" scoped>
.parent {
  margin-top: 100px;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  @media only screen and (max-width: 768px) {
    flex-direction: column;
    margin-top: 30px;
  }
}
img {
  width: 14vw;
  height: 20vw;
  @media only screen and (max-width: 768px) {
    width: 100%;
    height: 45vw;
    margin-top: 5px;
  }
}
.txt-parent {
  margin-top: -90px;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  position: relative;
  @media only screen and (max-width: 768px) {
    flex-direction: column;
    margin-top: 5px;
  }
}

.txt {
  width: 250px;
  height: 300px;
  background-color: white;
  transform-style: preserve-3d;
  transition: all 1s ease-in-out;
  border: 1px solid lightgray;
  box-shadow: 0 10px 20px -6px rgba(114, 113, 113, 0.623);
  &:hover {
    transform: rotateY(180deg);
  }
  @media only screen and (max-width: 768px) {
    text-align: center;
    height: auto;
    width: 100%;
    margin-top: 5px;
    padding-top:30px;
    padding-bottom:30px;
  }
}
.side {
  backface-visibility: hidden;
  border-radius: 6px;
  height: 100%;
  position: absolute;
  overflow: hidden;
  width: 100%;

}
.back {
  color: #28556b;
  line-height: 150px;
  font-size:25px;
  text-align: center;
  font-weight: 700;
  transform: rotateY(180deg);
}
h3 {
  font-size: 22px;
}
h5 {
  margin-top: 5px;
  color: orange;
  font-size: 14px;
}
p {
  margin-top: 20px;
  color: gray;
}
p,
h3,
h5 {
  padding-left: 10px;
}
</style>