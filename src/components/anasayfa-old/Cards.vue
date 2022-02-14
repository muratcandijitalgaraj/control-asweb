<template>
  <div class="bigContainer">
    <div class="cards">
      <div class="card card1">
        <img
          src="../../assets/anasayfa/randevu-alin.svg"
          alt=""
          class="cardLogo"
        />
        <div class="cardPara">Hastane Randevusu Alın</div>
      </div>
      <div class="card card2">
        <img
          src="../../assets/anasayfa/goruntulu.svg"
          alt=""
          class="cardLogo"
        />
        <div class="cardPara">Görüntülü Görüşme Randevusu Alın</div>
      </div>
      <div class="card card3">
        <img src="../../assets/anasayfa/check-up.svg" alt="" class="cardLogo" />
        <div class="cardPara">Check-Up Başvurusu Yapın</div>
      </div>
      <div class="card card4">
        <img src="../../assets/anasayfa/destek.svg" alt="" class="cardLogo" />
        <div class="cardPara">Destek Merkezi</div>
      </div>
    </div>
    <div class="greyLine"></div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.bigContainer {
  /* margin: 0;
  padding: 0; */
  width: 100%;
  display: flex;
  flex-direction: column;
  /* justify-content: center; */
  align-items: center;
  /* border: 1px solid red; */
  height: auto;
}
.cards {
  width: 100%;
  height: auto;
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: flex-start;
  /* border-bottom: 2px solid red; */
}
.greyLine {
  margin-top: 1rem;
  width: 90%;
  height: 0px;
  margin-bottom: 18px;
  border: 1px solid #dae9f1;
}
.cardContainer {
  display: flex;
  flex-direction: row;
  justify-content: space-evenly;
  align-items: flex-start;
  width: 100%;
  height: auto;
}
.card {
  height: 110px;
  width: 100%;
  margin: 15px;
  display: flex;
  justify-content: center;
  padding-left: 20px;
}
.card1 {
  border-top: 2px solid #32a5df;
}
.card2 {
  border-top: 2px solid #ff8038;
}
.card3 {
  border-top: 2px solid #7367f0;
}
.card4 {
  border-top: 2px solid #29a87b;
}
.cardLogo {
  width: 26px;
  height: 26px;
  margin-bottom: 10px;
}
.cardPara {
  width: 116px;
  height: 44px;

  /* menu */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 22px;

  /* Primary */
  color: #3c4e69;
}
@media only screen and (max-width: 1500px) {
  /* .cards {
    display: flex;
    flex-direction: column;
    justify-content: flex-start;
    align-items: center;
  } */
  .card {
    width: 210px;
    /* border: 2px solid black; */
  }
}
@media only screen and (max-width: 1000px) {
  /* .cards {
    flex-direction: column;
    justify-content: flex-start;
  } */
  .cardContainer {
    flex-direction: column;
    /* border: 2px solid red; */
    align-items: center;
  }
  .cards {
    flex-wrap: wrap;
  }
  .card {
    width: 210px;
    padding: 1rem;
  }
}
@media only screen and (max-width: 500px) {
  .card {
    width: auto;
  }
}
</style>
