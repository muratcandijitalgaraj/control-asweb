<template>
  <div class="sideBar">
    <div class="upperItem">
      <img src="../../assets/sidebar/foto.svg" alt="" class="foto" />
    </div>
    <div class="upperItem para">Akgül Yılmaz</div>
    <div class="greyLine"></div>
    <!-- <div class="item">
      <img src="" alt="" class="itemLogo">
      <div class="itemPara"></div>
    </div> -->
    <div class="item">
      <img src="../../assets/sidebar/giris.svg" alt="" class="itemLogo" />
      <div class="itemPara">Giriş</div>
    </div>
    <div class="item">
      <img
        src="../../assets/sidebar/randevularim.svg"
        alt=""
        class="itemLogo"
      />
      <div class="itemPara">Randevularım</div>
    </div>
    <div class="item">
      <img src="../../assets/sidebar/kayitlar.svg" alt="" class="itemLogo" />
      <div class="itemPara">Tıbbi Kayıtlar</div>
      <img src="../../assets/sidebar/1.svg" alt="" class="notification" />
    </div>
    <div class="item">
      <img src="../../assets/sidebar/gecmis.svg" alt="" class="itemLogo" />
      <div class="itemPara">Geçmiş Muayeneler</div>
    </div>
    <div class="item">
      <img src="../../assets/sidebar/receteler.svg" alt="" class="itemLogo" />
      <div class="itemPara">Reçeteler</div>
    </div>
    <div class="item">
      <img src="../../assets/sidebar/hesap.svg" alt="" class="itemLogo" />
      <div class="itemPara">Hesap Bilgileriniz</div>
    </div>
    <div class="item">
      <img src="../../assets/sidebar/anket.svg" alt="" class="itemLogo" />
      <div class="itemPara">Anketimize Katılın</div>
    </div>
    <div class="item">
      <img src="../../assets/sidebar/cikis.svg" alt="" class="itemLogo" />
      <div class="itemPara">Çıkış Yap</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.sideBar {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  /* border: 2px solid gold; */
  background: #f9fdff;
  border-top-left-radius: 18px;
  border-bottom-left-radius: 18px;
}
.greyLine {
  width: 210px;
  height: 0px;
  margin-bottom: 18px;
  border: 1px solid #dae9f1;
}
.upperItem {
  /* border: 1px solid black; */
  height: auto;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.foto {
  height: 116px;
  width: 116px;
  /* border: 1px solid black; */
  border-radius: 0px;
}
.para {
  width: 96px;
  height: 22px;
  left: 425px;
  top: 228px;

  /* menu */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 22px;
  /* identical to box height */

  text-align: center;

  /* Primary */

  color: #3c4e69;
  margin-bottom: 18px;
}
.item {
  height: auto;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  margin-bottom: 20px;
  /* border: 1px solid black; */
}
.itemLogo {
  width: 30px;
  height: 40px;
  margin-left: 30px;
  margin-right: 10px;
}
.itemPara {
  width: auto;
  height: 22px;

  /* menu */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 16px;
  line-height: 22px;
  /* identical to box height */

  /* Primary */

  color: #3c4e69;
  /* border: 1px solid red; */
}
.notification {
  width: 20px;
  height: 20px;
  margin-left: 5px;
}
</style>
