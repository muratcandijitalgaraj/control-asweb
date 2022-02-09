<template>
  <div class="cell">
    <div class="logoBox">
      <img src="../../assets/anasayfa/gorusme.svg" alt="" class="logo" />
    </div>
    <div class="boxes box1">
      <div class="boxTitle redTitle">Görüşme Bekleniyor</div>
      <div class="boxPara">20 Ocak Pazartesi - 12:30</div>
    </div>
    <!-- flex row -->
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
        <img src="../../assets/anasayfa/hospital.svg" alt="" class="greyLogo" />
      </div>
      <div class="boxes">
        <div class="boxTitle greyTitle">Ataşehir Tıp Merkezi</div>
        <div class="boxPara">Ataşehir Tıp Merkezi</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.cell {
  width: auto;
  height: auto;
  margin-left: 30px;
  margin-right: 30px;
  background: #ffffff;
  /* Boxx Shadow */

  box-shadow: 0px 1px 3px rgba(42, 49, 55, 0.11);
  border-radius: 10px;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
.logoBox {
  width: 40px;
  height: 100px;
  border-radius: 5px;
  margin-right: 30px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #ffeeee;
}
.greyBox {
  width: 50px;
  height: 50px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: #f2f8fb;
  border-radius: 5px;
}
.logo {
  height: 20px;
  width: auto;
  margin-left: 1rem;
  border-radius: 0px;
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
.boxes {
  /* border: 1px solid black; */
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
  display: flex;
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
@media only screen and (max-width: 1870px) {
  .cell {
    height: auto;
  }
  .boxes {
    /* border: 1px solid black; */
    width: auto;
    margin-bottom: 1rem;
  }
  .logoBox {
    width: 80%;
    height: 2rem;
  }
}
</style>
