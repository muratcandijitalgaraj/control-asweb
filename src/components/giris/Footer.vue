<template>
  <div class="footerComponent">
    <div class="container">
      <div class="flexContainer">
        <div class="logoPart">
          <div class="leftPart">
            <img
              src="../../assets/giris/logoGroup.svg"
              alt=""
              class="logoGroup"
            />
            <p class="footerPara">
              Anadolu Eğitim ve Sosyal Yardım Sağlık Tesisleri İktisadi
              İşletmesi, Vakıflar Kanunu’nun 26/1 maddesine göre tesis edilmiş
              bir vakıf işletmesidir.
            </p>
          </div>
          <div class="telefon">
            <img
              src="../../assets/giris/telefon.svg"
              alt=""
              class="telefonLogo"
            />
            <div class="telefonGroup">
              <div class="telefonText">
                Anadolu Grubu Danışma Hattı <br />
                <span class="telefonNo">+90 (262) 678 54 00</span>
              </div>
            </div>
          </div>
        </div>
        <div class="copyright">Copyright © 2018 Anadolu Sağlık Merkezi</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.footerComponent {
  width: auto;
  height: auto;
  background: #ffffff;
  /* border: 1px solid black; */
  display: flex;
  flex-direction: row;
  justify-content: center;
  margin-top: 20px;
  /* padding: 0  */
  padding-left: 2rem;
}
.container {
  width: 70%;
  height: auto;

  /* border: 10px solid black; */
}
.flexContainer {
  /* display: flex;
  flex-direction: column; */
}
.logoPart {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  border-bottom: 1px solid #f4f4f4;
}
.leftPart {
  display: flex;
}
.logoGroup {
  width: 238.21px;
  height: 40px;
  margin-right: 16px;
}
.footerPara {
  width: 446px;
  height: 34px;

  /* text4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 130%;
  /* or 17px */

  letter-spacing: -0.01em;

  /* Gri */

  color: #818b9a;
}
.telefon {
  width: auto;
  /* justify-self: flex-end; */
  /* border: 1px solid red; */
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: center;
}
.telefonGroup {
  height: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* border: 1px solid black; */
}
.telefonLogo {
  width: 30px;
  height: 30px;
  margin-right: 10px;
}
.telefonText {
  width: 184px;
  height: 34px;

  /* text4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 13px;
  line-height: 130%;
  /* or 17px */

  letter-spacing: -0.01em;

  /* Turuncu */

  color: #ff8038;
}
.telefonNo {
  width: 184px;
  height: 34px;

  /* text4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 130%;
  /* or 17px */

  letter-spacing: -0.01em;

  /* Gri */

  color: #818b9a;
}
.copyright {
  width: 248px;
  height: 17px;

  /* text4 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 13px;
  line-height: 130%;
  /* identical to box height, or 17px */

  letter-spacing: -0.01em;

  /* Gri */

  color: #818b9a;
  margin-top: 16px;
}
</style>
