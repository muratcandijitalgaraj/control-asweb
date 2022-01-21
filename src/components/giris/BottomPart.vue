<template>
  <div class="bottomPartComponent">
    <div class="greySpace"></div>
    <img class="frame" src="../../assets/giris/frame.svg" alt="" />
    <div class="itemContainer">
      <div class="textGroup">
        <p class="blueText">
          Mobil Uygulamamız ile Anadolu Sağlık hizmetlerine
          <span class="orangeText">her yerden ulaşın</span>
        </p>
        <img class="arrow" src="../../assets/giris/arrow.svg" alt="" />
      </div>
      <div class="downloadButtons">
        <button class="appleBtn"></button>
        <button class="googleBtn"></button>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.bottomPartComponent {
  height: 100%;
  width: 100%;
  /* border: 1px solid red; */
  margin-top: 24rem;
  display: flex;
  flex-direction: column;
}
.greySpace {
  background: #e9f3f9;

  height: 3.5rem;
}
.itemContainer {
  width: 100%;
  height: 9rem;
  display: flex;
  background: #f3fafe;
}
.frame {
  position: absolute;
  width: 250px;
  height: 190px;
  /* border: 3px solid red; */
  left: 20rem;
}
.textGroup {
  /* border: 1px solid red; */
  width: 439px;
  display: flex;
  align-items: center;
  margin-left: 38em;
}
.blueText {
  width: 439px;
  height: 52px;

  /* baslik-alt2 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 130%;
  /* or 26px */

  letter-spacing: -0.01em;

  /* Secondary */

  color: #32a5df;
}
.orangeText {
  width: 439px;
  height: 52px;

  /* baslik-alt2 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 20px;
  line-height: 130%;
  /* or 26px */

  letter-spacing: -0.01em;

  /* Turuncu */

  color: #ff8038;
}
.arrow {
  /* Turuncu */
  width: 92px;
  height: 33px;
  /* background: #ff8038; */
  /* transform: matrix(-0.99, 0.12, 0.12, 0.99, 0, 0); */
  position: relative;
  /* left: 5rem; */
  /* top: 10rem; */
  right: 2rem;
  top: 1em;
}
.appleBtn,
.googleBtn {
  width: 195px;
  height: 60px;

  /* Secondary */

  background: #32a5df;
  border-radius: 40px;
  margin-right: 30px;
}
.downloadButtons {
  display: flex;
  flex-direction: row;
  align-items: center;
}
</style>
