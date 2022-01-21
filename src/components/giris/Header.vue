<template>
  <div class="girisHeader">
    <div class="container">
      <div class="logoPart">
        <img class="logo" src="../../assets/giris/logo.svg" alt="" />
        <div class="islemler">ONLINE İŞLEMLER</div>
      </div>
      <div class="signupPart">
        <div class="signupPara">Henüz üye değil misiniz?</div>
        <button class="signupBtn">Kayıt Olun</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.girisHeader {
  height: auto;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: center;
  /* border: 1px solid red; */
  padding-top: 30px;
}
.container {
  height: auto;
  width: 70%;
  /* border: 1px solid black; */
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
}
.logoPart {
  width: 100%;
  height: auto;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  /* margin-top: 30px; */
}
.logo {
  width: auto;
  height: auto;
  /* border: 1px solid red; */
  margin-right: 1.458rem;
}
.islemler {
  width: auto;
  height: auto;

  /* text3 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* or 21px */

  letter-spacing: -0.01em;

  color: #ffffff;
}
.signupPart {
  height: 100%;
  width: 100%;
  /* border: 1px solid red; */
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  /* margin-top: 30px; */
}
.signupPara {
  width: 171px;
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
}
.signupBtn {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 12px 20px 11px;

  width: 114px;
  height: 40px;

  /* Beyaz */

  background: #ffffff;
  border-radius: 6px;
  border: none;
  color: #ff7c32;

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

  /* Button Primary */

  color: #ff7c32;

  /* Inside auto layout */

  flex: none;
  order: 0;
  flex-grow: 0;
  margin: 0px 10px;
}
</style>
