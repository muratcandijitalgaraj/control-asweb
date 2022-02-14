<template>
  <b-row class="d-flex justify-content-around cards">
    <b-col cols="12" lg="6" xl="3" class="card card1">
      <img
        src="../../assets/anasayfa/randevu-alin.svg"
        alt=""
        class="cardLogo"
      />
      <div class="cardPara">Hastane Randevusu Alın</div></b-col
    >
    <b-col cols="12" lg="6" xl="3" class="card card2">
      <img src="../../assets/anasayfa/goruntulu.svg" alt="" class="cardLogo" />
      <div class="cardPara">Görüntülü Görüşme Randevusu Alın</div></b-col
    >
    <b-col cols="12" lg="6" xl="3" class="card card3">
      <img src="../../assets/anasayfa/check-up.svg" alt="" class="cardLogo" />
      <div class="cardPara">Check-Up Başvurusu Yapın</div></b-col
    >
    <b-col cols="12" lg="6" xl="3" class="card card4">
      <img src="../../assets/anasayfa/destek.svg" alt="" class="cardLogo" />
      <div class="cardPara">Destek Merkezi</div></b-col
    >
  </b-row>
</template>

<script>
export default {};
</script>

<style scoped>
.cards {
  width: auto;
}
.card {
  min-height: 110px;
  width: 210px;
  margin-bottom: 1rem;
  margin-top: 1rem;
  margin-left: 1rem;
  display: flex;
  justify-content: center;
  /* 
 

  
  padding-left: 20px;
  margin-right: 10px;
  margin-bottom: 1rem;
  margin-top: 1rem; */
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
  width: auto;
  height: auto;

  /* menu */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 22px;

  /* Primary */
  color: #3c4e69;
  /* margin-bottom: 2rem; */
}
.greyLine {
  margin-top: 1rem;
  width: 100%;
  height: 0px;
  margin-bottom: 18px;
  border: 1px solid #dae9f1;
}
</style>
