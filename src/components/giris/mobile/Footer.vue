<template>
  <div class="footerComponent">
    <div class="container">
      <img
        src="../../../assets/giris/logoGroup.svg"
        alt=""
        class="logoGroup item"
      />
      <p class="footerPara item">
        Anadolu Eğitim ve Sosyal Yardım Sağlık Tesisleri İktisadi İşletmesi,
        Vakıflar Kanunu’nun 26/1 maddesine göre tesis edilmiş bir vakıf
        işletmesidir.
      </p>
      <div class="telefon item">
        <img
          src="../../../assets/giris/telefon.svg"
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
      <div class="copyright item">Copyright © 2018 Anadolu Sağlık Merkezi</div>
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
  /* margin-top: 20px; */
  /* padding: 0  */
  padding-left: 2rem;
  padding-top: 1rem;
  padding-bottom: 0.5rem;
  margin-top: 8em;
}
.container {
  width: 70%;
  height: auto;
  align-self: flex-end;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  /* border: 10px solid black; */
}
.item {
  margin-bottom: 1rem;
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
  width: auto;
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
  margin-bottom: 3.5rem;
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
