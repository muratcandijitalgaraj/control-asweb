<template>
  <div class="sideBar">
    <div class="top">
      <div class="upperItem">
        <img src="../../assets/sidebar/foto.svg" alt="" class="foto" />
      </div>
      <!-- <div class="upperItem para">Akgül Yılmaz</div> -->
      <!-- collapse for mobile -->

      <button
        v-b-toggle.collapse-1
        variant="primary"
        class="collapsable upperItem para profileButton"
      >
        Akgül Yılmaz
      </button>
      <b-collapse id="collapse-1" class="mt-2">
        <b-card class="card">
          <span class="item">
            <img src="../../assets/sidebar/giris.svg" alt="" class="itemLogo" />
            <span class="itemPara">Giriş</span>
          </span>
          <div class="item">
            <img
              src="../../assets/sidebar/randevularim.svg"
              alt=""
              class="itemLogo"
            />
            <div class="itemPara">Randevularım</div>
          </div>
          <div class="item">
            <img
              src="../../assets/sidebar/kayitlar.svg"
              alt=""
              class="itemLogo"
            />
            <div class="itemPara">
              Tıbbi Kayıtlar
              <img
                src="../../assets/sidebar/1.svg"
                alt=""
                class="notification"
              />
            </div>
          </div>
          <div class="item">
            <img
              src="../../assets/sidebar/gecmis.svg"
              alt=""
              class="itemLogo"
            />
            <div class="itemPara">Geçmiş Muayeneler</div>
          </div>
          <div class="item">
            <img
              src="../../assets/sidebar/receteler.svg"
              alt=""
              class="itemLogo"
            />
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
        </b-card>
      </b-collapse>
    </div>
    <div class="greyLine"></div>

    <div class="container hideInMobile">
      <div class="bigItemContainer">
        <div class="itemContainer">
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
        </div>
        <div class="itemContainer">
          <div class="item">
            <img
              src="../../assets/sidebar/kayitlar.svg"
              alt=""
              class="itemLogo"
            />
            <div class="itemPara">Tıbbi Kayıtlar</div>
          </div>
          <div class="item">
            <img
              src="../../assets/sidebar/gecmis.svg"
              alt=""
              class="itemLogo"
            />
            <div class="itemPara">Geçmiş Muayeneler</div>
          </div>
        </div>
      </div>
      <div class="bigItemContainer">
        <div class="itemContainer">
          <div class="item">
            <img
              src="../../assets/sidebar/receteler.svg"
              alt=""
              class="itemLogo"
            />
            <div class="itemPara">Reçeteler</div>
          </div>
          <div class="item">
            <img src="../../assets/sidebar/hesap.svg" alt="" class="itemLogo" />
            <div class="itemPara">Hesap Bilgileriniz</div>
          </div>
        </div>
        <div class="itemContainer">
          <div class="item">
            <img src="../../assets/sidebar/anket.svg" alt="" class="itemLogo" />
            <div class="itemPara">Anketimize Katılın</div>
          </div>
          <div class="item">
            <img src="../../assets/sidebar/cikis.svg" alt="" class="itemLogo" />
            <div class="itemPara">Çıkış Yap</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.sideBar {
  height: 270px;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  /* border: 2px solid gold; */
  background: #f9fdff;
  border-top-left-radius: 18px;
  border-top-right-radius: 18px;
  /* flex-wrap: wrap; */
}
.collapsable {
  display: none;
}
.container {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: row;
  /* border: 2px solid gold; */
}
.bigItemContainer {
  display: flex;
  width: 100%;
  height: 100%;
}
.top {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* border: 1px solid red; */
  width: auto;
}
.greyLine {
  width: 0px;
  height: 210px;

  border: 1px solid #dae9f1;
}
.itemContainer {
  width: 100%;
  height: 100%;

  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.item {
  display: flex;
  justify-content: flex-start;
}
.itemPara {
  width: auto;
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
  margin-bottom: 10px;
  /* border: 1px solid black; */
}
.itemLogo {
  width: 30px;
  height: 40px;
  margin-left: 10px;
  margin-right: 10px;
}
/* .item{
    width: 200px;

} */
.itemPara {
  width: 200px;
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
@media only screen and (max-width: 1700px) {
  .container {
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    /* border: 2px solid red; */
  }
  .sideBar {
    height: 100%;
    width: 100%;
    flex-direction: column;
  }
  .greyLine {
    width: 210px;
    height: 0px;

    border: 1px solid #dae9f1;
  }
  .hideInMobile {
    display: none;
  }
  .container {
    /* border: 2px solid black; */
  }
  .profileButton {
    height: auto;
    width: auto;
    border: none;
    padding: 5px;
    border-radius: 5%;
  }
}
/* @media only screen and (max-width: 1200px) {
}
@media only screen and (max-width: 915px) {
  .sideBar {
    height: 100%;
    width: 100%;
    flex-direction: column;
  }
  .greyLine {
    width: 210px;
    height: 0px;

    border: 1px solid #dae9f1;
  }
  .hideInMobile {
    display: none;
  }

} */
@media only screen and (max-width: 750px) {
  .collapsable {
    display: block;
  }
  .hideInMobile {
    display: none;
  }
  .card {
    height: auto;
    margin: 0;
    width: 100%;
    /* border: 2px solid black; */
    background: #f9fdff;
    padding: 0;
    border: none !important;
  }
  .mt-2 {
    margin: 0;
    padding: 0;
    width: 100%;
    /* border: 2px solid red; */
  }
}
</style>
