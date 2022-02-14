<template>
  <div class="anasayfaHeader">
    <div class="headerLogoPart">
      <img src="../../assets/giris/logo.svg" alt="" class="logo" />
      <div class="headerIslemler">ONLINE İŞLEMLER</div>
    </div>
    <div class="notifications">
      <img
        src="../../assets/anasayfa/notifications.svg"
        alt=""
        class="notification bell"
      />
      <img
        src="../../assets/anasayfa/bildirim.svg"
        alt=""
        class="notification picture"
      />
      <div class="notificationPara">Profil Değiştir</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.anasayfaHeader {
  height: 100%;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  padding: 0 2rem;
  margin: 0;
}
.container {
  height: 100%;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  border: solid;
  padding: 0;
  margin: 0;
}
.headerLogoPart {
  margin-top: 25px;
}
.logo {
  width: auto;
  height: auto;
}
.headerIslemler {
  height: 42px;
  width: 69px;
  border-radius: nullpx;
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
.notifications {
  margin-top: 38px;
  height: 2.5rem;
  width: auto;
  border-radius: 0px;
  display: flex;
  justify-content: flex-end;
  align-items: center;
  /* border: 2px solid black; */
}
.bell {
  border-right: 1px solid rgba(0, 0, 0, 0.1);
  padding-right: 1rem;
}
.picture {
  padding-left: 1rem;
  padding-right: 1rem;
}
.notification {
  /* border: 2px solid black; */
  width: auto;
}
.notificationPara {
  width: auto;
  /* border: 1px solid black; */
  /* text4-bold */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 13px;
  line-height: 130%;
  /* identical to box height, or 17px */

  text-align: right;
  letter-spacing: -0.01em;
  display: flex;
  align-items: center;
  color: #ffffff;
}

@media only screen and (max-width: 900px) {
  .anasayfaHeader {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
}
</style>
