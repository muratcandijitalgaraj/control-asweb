<template>
  <div class="tallCell">
    <div class="rightPart">
      <div class="top">
        <div class="boxes box1">
          <div class="boxTitle orangeTitle">20 OCAK 2021 - 12:30</div>
          <div class="boxPara">Ataşehir Tıp Merkezi</div>
        </div>
        <div class="boxes box2">
          <img src="../../assets/anasayfa/doktor.svg" alt="" class="doktor" />
          <!-- flex column -->
          <div class="textGroup">
            <div class="boxTitle">Prof. Dr. Mehmet Ali Tahaoğlu</div>
            <div class="boxPara">Gögüs Hastalıkları</div>
          </div>
        </div>
        <div class="boxes box3">
          <div class="icons">
            <img src="../../assets/anasayfa/lab.svg" alt="" class="icon" />
            <img
              src="../../assets/anasayfa/radyoloji.svg"
              alt=""
              class="icon"
            />
            <img src="../../assets/anasayfa/patoloji.svg" alt="" class="icon" />
            <img src="../../assets/anasayfa/recete.svg" alt="" class="icon" />
          </div>
        </div>
      </div>
      <div class="greyLine"></div>
      <div class="bottom">
        <!-- flex row -->
        <div class="bottomPara">
          <div class="paraItem">
            <img src="../../assets/anasayfa/star.svg" alt="" class="icon" />
            <div class="paraText">Puan Ver</div>
          </div>
          <div class="paraItem">
            <img src="../../assets/anasayfa/story.svg" alt="" class="icon" />
            <div class="paraText">Ankete Katıl</div>
          </div>
        </div>
        <button class="bottomButton">
          <div class="buttonPara">Randevu Alın</div>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.tallCell {
  height: auto;
  width: auto;
  background: #ffffff;
  margin-left: 30px;
  margin-right: 30px;
  box-shadow: 0px 1px 3px rgba(42, 49, 55, 0.11);
  border-radius: 10px;
  display: flex;
}
.greyLine {
  width: 80%;
  height: 1px;
  background: #f3f3f3;

  /* margin-top: 30px;
  margin-bottom: 25px; */
}

.rightPart {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.top {
  width: 100%;
  height: auto;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
  margin-top: 30px;
  padding-left: 20px;
  padding-right: 30px;
}
.boxes {
  height: auto;
  width: auto;
  margin-right: 2rem;
}
.box1 {
  width: 171px;
}
.box2 {
  width: 292px;
  display: flex;
}
.box3 {
  /* border: 1px solid black; */
  display: flex;
  /* justify-content: center; */
}

.redTitle {
  /* Kırmızı */
  color: #ea5455;
}
.doktor {
  width: 50px;
  height: 50px;
  margin-right: 1rem;
}
.textGroup {
  display: flex;
  flex-direction: column;
}
.greyLogo {
  width: 22px;
  height: 22px;
  margin-right: 1rem;
}
.boxTitle {
  width: auto;
  height: 24px;

  /* baslik4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;
  /* identical to box height, or 24px */
}
.boxPara {
  /* text3 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* identical to box height, or 21px */

  letter-spacing: -0.01em;

  /* Primary */

  color: #3c4e69;
}
.orangeTitle {
  /* Kırmızı */
  color: #ff8038;
}
.greyTitle {
  width: 148px;
  height: 48px;
}

.bottom {
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  /* height: auto; */
  padding-left: 20px;
  padding-right: 50px;
  padding-top: 15px;
  padding-bottom: 15px;

  /* border: 2px solid black; */
}
.bottomPara {
  width: auto;
  height: auto;
  display: flex;
  justify-content: center;
  align-items: center;

  /* text3 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* identical to box height, or 21px */

  letter-spacing: -0.01em;

  color: #818b9a;
}
.paraItem {
  width: auto;
  height: auto;
  margin-right: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
}
.paraText {
  width: auto;
  height: auto;
  margin-left: 8px;
}
.bottomButton {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 12px 20px 11px;

  width: 250px;
  height: 40px;

  /* Button Primary */

  background: #ff7c32;
  border: none;
  border-radius: 6px;
}
.buttonPara {
  width: auto;
  height: 17px;

  /* buton-text-kucuk */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 15px;
  line-height: 110%;
  /* identical to box height, or 17px */

  display: flex;
  align-items: center;
  text-align: center;

  /* Beyaz */

  color: #ffffff;

  /* Inside auto layout */

  flex: none;
  order: 0;
  flex-grow: 0;
  margin: 0px 10px;
}
.icons {
  /* border: 1px solid black; */
  width: 224px;
  height: 43px;
  display: flex;
  justify-content: space-evenly;
  align-items: center;
}
.icon {
  width: 20px;
  height: 20px;
}
@media only screen and (max-width: 1250px) {
  .tallCell {
    flex-direction: column;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
  }
  .bottom {
    flex-direction: column;
  }
  .bottomPara {
    margin-bottom: 10px;
  }
}
</style>
