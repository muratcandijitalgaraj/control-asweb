<template>
  <b-row class="d-flex justify-content-around cell">
    <b-col class="logoBox" cols="1">
      <img src="../../assets/anasayfa/gorusme.svg" alt="" class="logo" />
    </b-col>
    <b-col class="boxContainer">
      <div class="boxes">
        <div class="boxTitle redTitle">Görüşme Bekleniyor</div>
        <div class="boxPara">20 Ocak Pazartesi - 12:30</div>
      </div>
    </b-col>
    <b-col>
      <div class="boxContainer">
        <img src="../../assets/anasayfa/doktor.svg" alt="" class="doktor" />
        <!-- flex column -->
        <div class="boxes">
          <div class="boxTitle">Prof. Dr. Mehmet Ali Tahaoğlu</div>
          <div class="boxPara">Gögüs Hastalıkları</div>
        </div>
      </div></b-col
    >
    <b-col>
      <div class="boxContainer">
        <div class="greyBox">
          <img
            src="../../assets/anasayfa/hospital.svg"
            alt=""
            class="greyLogo"
          />
        </div>
        <div class="boxes">
          <div class="boxTitle greyTitle">Ataşehir Tıp Merkezi</div>
          <div class="boxPara">Ataşehir Tıp Merkezi</div>
        </div>
      </div></b-col
    >
  </b-row>
</template>

<script>
export default {};
</script>

<style scoped>
.cell {
  width: auto;
  min-height: 110px;
  height: auto;

  background: #ffffff;
  /* Boxx Shadow */

  box-shadow: 0px 1px 3px rgba(42, 49, 55, 0.11);
  border-radius: 10px;
}
.boxes {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
}
.boxContainer {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100px;
  padding: 0;
}
.doktor {
  width: 50px;
  height: 50px;
  margin-right: 1rem;
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
.redTitle {
  /* Kırmızı */
  color: #ea5455;
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
.logoBox {
  width: 40px;
  height: auto;
  background: #ffeeee;
  border-radius: 5px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.logo {
  height: 20px;
  width: 20px;
  /* margin-left: 1rem; */
  border-radius: 0px;
  margin: 0;
}
</style>
