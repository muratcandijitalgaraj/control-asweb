<template>
  <div class="tallCell">
    <!-- tablet design -->
    <div class="showOnTablet">
      <div class="rightPart">
        <div class="top">
          <div class="boxes box1">
            <div class="logoBox">
              <img src="../../assets/anasayfa/odeme.svg" alt="" class="logo" />
            </div>
            <div class="boxTexts">
              <div class="boxTitle orangeTitle">Görüşme Bekleniyor</div>
              <div class="boxPara">20 Ocak Pazartesi - 12:30</div>
            </div>
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
            <div class="greyBox">
              <img
                src="../../assets/anasayfa/hospital.svg"
                alt=""
                class="greyLogo"
              />
            </div>
            <div class="boxes">
              <div class="boxTitle greyTitle">Görüntülü Görüşme Randevusu</div>
            </div>
          </div>
        </div>
        <div class="greyLine"></div>
        <div class="bottom">
          <div class="bottomPara">
            Ödemenizi yaptığınızda randevunuz aktif hale gelecektir.
          </div>
          <button class="bottomButton">
            <div class="buttonPara">241 TL Ödeme Yapın</div>
          </button>
        </div>
      </div>
    </div>

    <!-- desktop design -->
    <div class="logoBox showOnDesktop">
      <img src="../../assets/anasayfa/odeme.svg" alt="" class="logo" />
    </div>
    <div class="rightPart showOnDesktop">
      <div class="top">
        <div class="boxes box1">
          <div class="boxTitle orangeTitle">Görüşme Bekleniyor</div>
          <div class="boxPara">20 Ocak Pazartesi - 12:30</div>
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
          <div class="greyBox">
            <img
              src="../../assets/anasayfa/hospital.svg"
              alt=""
              class="greyLogo"
            />
          </div>
          <div class="boxes">
            <div class="boxTitle greyTitle">Görüntülü Görüşme Randevusu</div>
          </div>
        </div>
      </div>
      <div class="greyLine"></div>
      <div class="bottom">
        <div class="bottomPara">
          Ödemenizi yaptığınızda randevunuz aktif hale gelecektir.
        </div>
        <button class="bottomButton">
          <div class="buttonPara">241 TL Ödeme Yapın</div>
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
  /* border: 2px solid black; */
}
.showOnTablet {
  display: none;
}
.greyLine {
  width: 80%;
  height: 1px;
  background: #f3f3f3;

  /* margin-top: 30px;
  margin-bottom: 25px; */
}
.logoBox {
  width: 40px;
  height: 170px;

  background: #fff9f0;
  border-radius: 5px;
  display: flex;
  align-items: flex-start;
  justify-content: center;
}
.logo {
  height: 20px;
  width: auto;
  margin-left: 1rem;
  border-radius: 0px;
  margin-top: 2.5rem;
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
  justify-content: space-between;
  align-items: center;
  flex-wrap: wrap;
  margin-top: 30px;
  padding-left: 25px;
  padding-right: 25px;
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
.orangeTitle {
  /* Kırmızı */
  color: #ff8038;
}
.greyTitle {
  width: 148px;
  height: 48px;
}
.greyBox {
  width: 50px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #f2f8fb;
  border-radius: 5px;
  margin-right: 15px;
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
  width: 145px;
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
.boxPara {
  width: 171px;
  height: 21px;

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
@media only screen and (max-width: 1250px) {
  .tallCell {
    /* flex-direction: column;
    justify-content: center;
    align-items: center; */
  }
  .top {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .bottom {
    flex-direction: column;
  }
  .boxes {
    /* border: 1px solid black; */
    width: auto;
    margin-bottom: 1rem;
  }
  .box1 {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .logoBox {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 50px;
    height: 50px;
    border-radius: 5px;
    margin-right: 15px;
  }
  .logo {
    height: 20px;
    width: 20px;
    margin: 0;
  }

  .showOnDesktop {
    display: none;
  }
  .showOnTablet {
    display: block;
  }
}
/* @media only screen and (max-width: 1250px) {
  .top {
    justify-content: center;
    padding-left: 0;
    padding-right: 0;
  }
}
@media only screen and (max-width: 400px) {
  .boxTitle {
    margin-bottom: 2rem;
  }
  .box2 {
    margin-left: 1rem;
  }
} */
</style>
