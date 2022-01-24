<template>
  <div class="bottomPart">
    <div class="greyPart"></div>
    <div class="mainPart">
      <div class="framePart">
        <img class="frame" src="../../../assets/giris/frame.svg" alt="" />
        <div class="textGroup">
          <div class="blueText">
            Mobil Uygulamamız ile Anadolu Sağlık

            <br />
            <div class="textWithArrow">
              <div class="blueText">
                hizmetlerine <span class="orangeText">her yerden ulaşın</span>
              </div>
              <!-- <img src="../../../assets/giris/arrow.svg" alt="" class="arrow" /> -->
            </div>
          </div>
          <div class="buttons">
            <button class="btn">
              <img
                src="../../../assets/giris/apple-logo.svg"
                alt=""
                class="btnLogo"
              />
              <div class="btnTextContainer">
                <div class="btnParaTop">
                  Hemen İndirin <br />
                  <div class="btnParaDown">App Store</div>
                </div>
              </div>
            </button>
            <button class="btn">
              <img
                src="../../../assets/giris/google-logo.svg"
                alt=""
                class="btnLogo"
              />
              <div class="btnTextContainer">
                <div class="btnParaTop">
                  Hemen İndirin <br />
                  <div class="btnParaDown">Google Play</div>
                </div>
              </div>
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.bottomPart {
  height: 250px;
  /* border: 1px solid black; */
  width: 100%;
  /* margin-top: 20rem; */
}
.greyPart {
  background: #e9f3f9;

  height: 3.5rem;
}
.mainPart {
  height: 140px;
  width: auto;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* padding-right: 20rem; */
  background: #f3fafe;
  /* border: 1px solid red; */
}
.framePart {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: auto;
  /* border: 1px solid red; */
  /* margin-bottom: 4rem; */
  background: #f3fafe;
}
.frame {
  width: 250px;
  overflow: visible;
  height: 190px;
  margin-right: 48px;
  /* background: black; */
}
/* .wrapGroup {
  width: auto;
  display: flex;
  flex-direction: row;
  justify-content: center;
} */
.textGroup {
  width: auto;
  height: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  /* border: 5px solid black; */
  /* flex-wrap: wrap; */
  /* padding-top: 4rem; */
}
.textWithArrow {
  width: auto;
  height: auto;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  /* border: 1px solid red; */
}
.blueText {
  /* border: 1px solid blue; */
  width: auto;
  height: 52px;
  margin-bottom: 1.5rem;

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
  height: 52px;

  /* baslik-alt2 */
  margin-right: 3rem;
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
/* .arrow {
  width: 92px;
  height: 33px;
  justify-self: flex-end;
  margin-right: 30px;
} */
.buttons {
  height: 100%;
  width: 100%;
  /* border: 2px solid black; */
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  background: #f3fafe;
  /* padding-top: 2rem; */
}
.btn {
  /* Rectangle 6 */
  width: 12.188rem;
  height: 3.75rem;
  /* Secondary */
  background: #32a5df;
  border-radius: 40px;
  border: none;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  /* border: 2px solid black; */
  margin-right: 30px;
}
.btnLogo {
  width: 24.75px;
  height: 30px;
  padding-left: 1rem;
}
.btnTextContainer {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
  /* border: 1px solid red; */
  /* padding-bottom: 1.5rem;
  padding-left: 1rem; */
  width: 100%;
  height: 100%;
  padding-left: 1rem;
  padding-bottom: 1rem;
}
.btnParaTop {
  width: auto;
  height: 17px;

  /* text4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 130%;
  /* identical to box height, or 17px */
  /* border: 1px solid black; */
  letter-spacing: -0.01em;

  color: #ffffff;
}
.btnParaDown {
  width: auto;
  height: 24px;

  /* baslik4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;

  color: #ffffff;
  /* border: 1px solid black; */
}
</style>
