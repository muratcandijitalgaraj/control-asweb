<template>
  <div class="tallCell">
    <div class="logoBox">
      <img src="../../assets/anasayfa/odeme.svg" alt="" class="logo" />
    </div>
    <b-row class="d-flex justify-content-around cell no-gutters">
      <!-- <b-col cols="12" lg="1" xl="1" md="12" class="container no-gutters mx-0">
        <div class="logoBox">
          <img src="../../assets/anasayfa/gorusme.svg" alt="" class="logo" />
        </div>
      </b-col> -->
      <b-col cols="12" lg="6" xl="3" class="container">
        <div class="boxes">
          <div class="boxTitle redTitle">Ödeme Bekleniyor</div>
          <div class="boxPara">20 Ocak Pazartesi - 12:30</div>
        </div></b-col
      >
      <b-col cols="12" lg="6" xl="4" class="container">
        <div class="boxContainer">
          <img src="../../assets/anasayfa/doktor.svg" alt="" class="doktor" />
          <!-- flex column -->
          <div class="boxes">
            <div class="boxTitle">Prof. Dr. Mehmet Ali Tahaoğlu</div>
            <div class="boxPara">Gögüs Hastalıkları</div>
          </div>
        </div></b-col
      >
      <b-col cols="12" lg="12" xl="4" class="container">
        <div class="boxContainer">
          <div class="greyBox">
            <img
              src="../../assets/anasayfa/video.svg"
              alt=""
              class="greyLogo"
            />
          </div>
          <div class="boxes">
            <div class="boxTitle greyTitle">Görüntülü Görüşme Randevusu</div>
          </div>
        </div></b-col
      >
      <div class="greyLine"></div>
      <b-row class="bottomPart">
        <b-col cols="12" md="6" class="bottomPara d-flex justify-content-start"
          >Ödemenizi yaptığınızda randevunuz aktif hale gelecektir.</b-col
        >
        <b-col cols="12" md="6" class="bottomButton d-flex justify-content-end"
          ><button class="btn">
            <p class="buttonPara">241 Tl Ödeme Yapın</p>
          </button></b-col
        >
      </b-row>
    </b-row>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.tallCell {
  display: flex;
  margin-left: 12px;
  background: #ffffff;
  /* Boxx Shadow */
  box-shadow: 0px 1px 3px rgba(42, 49, 55, 0.11);
  border-radius: 10px;
  margin-bottom: 20px;
  margin-top: 20px;
  height: auto;
}
.greyLine {
  height: 1px;
  width: 90%;
  background: #dae9f1;
  margin-top: 20px;
  margin-bottom: 15px;
}
.cell {
  padding: 1rem;
  min-height: 180px;
  display: flex;
}
.container {
  height: 100px;
  height: auto;
  padding: 0;
  margin: 0;
}
.logoBox {
  width: 40px;
  height: 170px;
  background: #fff9f0;
  border-radius: 5px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 0;
  margin-right: 20px;
  align-self: center;
  margin-left: 5px;
}
.logo {
  height: 20px;
  width: 20px;
  /* margin-left: 1rem; */
  border-radius: 0px;
  margin: 0;
}
.boxes {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
}
.boxTitle {
  width: auto;
  height: auto;

  /* baslik4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;
  /* identical to box height, or 24px */
}
.greyTitle {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 150%;
  /* identical to box height, or 24px */

  /* Primary */

  color: #3c4e69;
}
.boxPara {
  width: auto;
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
.redTitle {
  /* Kırmızı */
  color: #ea5455;
}
.boxContainer {
  display: flex;
  width: auto;
  justify-content: flex-end;
  align-items: center;
  min-height: auto;
  height: 100%;
  padding: 0;
  margin-bottom: 2rem;
}
.doktor {
  width: 50px;
  height: 50px;
  margin-right: 1rem;
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
  /* this padding makes sure that the logo fits well */
  padding: 10px;
}
.greyLogo {
  width: 22px;
  height: 22px;
  margin-right: 1rem;
}
.bottomPara {
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* identical to box height, or 21px */

  letter-spacing: -0.01em;

  /* Gri */

  color: #818b9a;
  padding: 0;
}
.bottomPart {
  padding: 0;
  margin: 0;
}
.bottomButton {
}
.btn {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 12px 20px 11px;

  width: 250px;
  height: 40px;

  /* Button Primary */

  background: #ff7c32;
  border-radius: 6px;
}
.buttonPara {
  /* buton-text-kucuk */
  width: auto;
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
@media (max-width: 1200px) {
  .tallCell {
    flex-direction: column;
  }

  .boxContainer {
    align-items: center;
  }
  .boxes {
    /* align-items: center; */
  }
  .logoBox {
    width: 100%;
    height: auto;
    padding: 10px;
    margin: 0;
  }
}
@media (max-width: 1000px) {
  .container {
    margin-left: 1rem;
  }
}

@media (min-width: 1400px) {
  .bottomButton {
    padding-right: 3rem;
  }
}
</style>
