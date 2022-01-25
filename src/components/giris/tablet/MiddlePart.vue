<template>
  <div class="middlePartComponent">
    <div class="container">
      <div class="loginPart">
        <div class="loginTitles">
          <div class="hosgeldiniz">Hoşgeldiniz</div>
          <div class="giris">Giriş Yapın</div>
        </div>
        <div class="loginBox">
          <form @submit="changeControl" action="">
            <div class="inputs">
              <div class="telBox">
                <!-- <div class="inputCheck"> -->
                <input placeholder="+90" type="number" class="countryCode" />
                <!-- 
                  <span class="errorMsg" v-if="control"></span>
                </div> -->
                <div class="inputCheck">
                  <input
                    type="number"
                    class="telNo"
                    placeholder="Telefon Numaranız"
                  />
                  <span class="errorMsg" v-if="control"
                    >Geçerli bir telefon numarası yazın</span
                  >
                </div>
              </div>
              <div class="inputCheck">
                <input placeholder="Şifreniz" type="password" class="sifre" />
                <span class="errorMsg" v-if="control"
                  >Hatalı şifre girdiniz</span
                >
              </div>
            </div>

            <!-- space between here -->
            <div class="loginActions">
              <div class="hatirlaContainer">
                <img
                  src="../../../assets/giris/check-dolu.svg"
                  alt=""
                  class="hatirlaLogo"
                />
                <div class="hatirlaPara">Beni Hatırla</div>
              </div>
              <div class="unuttumContainer">
                <img
                  src="../../../assets/giris/flash-circle-1.svg"
                  alt=""
                  class="unuttumLogo"
                />
                <div class="unuttumPara">Şifremi Unuttum</div>
              </div>
            </div>
            <button class="loginBtn">Tamam</button>
          </form>
        </div>
      </div>
      <div class="carouselContainer">
        <img
          src="../../../assets/giris/orta-bulut.svg"
          alt=""
          class="orta-bulut"
        />
        <img
          src="../../../assets/giris/imageGroup-1.svg"
          alt=""
          class="carousel-image"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      control: false,
    };
  },
  methods: {
    changeControl: function (e) {
      e.preventDefault();
      this.control = true;
    },
  },
};
</script>

<style scoped>
.middlePartComponent {
  /* will change this */
  /* margin-top: 70px; */
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* border: 1px solid red; */
}
.container {
  height: 100%;
  width: 70%;
  /* display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: flex-end; */
  /* border: 10px solid red; */
}
.carouselContainer {
  width: 100%;
  height: 100%;
  /* border: 1px solid red; */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* position: absolute; */
}
.orta-bulut {
  /* width: auto;
  height: auto;
  position: absolute;
  top: 72px;

  margin-top: 5em; */
  padding: 0;
  width: auto;
  margin-top: 2rem;
  /* border: 1px solid red; */
}
.carousel-image {
  /* border: 1px solid red; */
  /* position: absolute;
  margin-top: 6.5em;
  top: 375; */
  width: auto;
  height: auto;
}
.loginPart {
  /* border: 1px solid black; */
  /* border: 1px solid black; */

  height: auto;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.loginTitles {
  /* border: 1px solid red; */
  height: auto;
  width: 468px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.hosgeldiniz {
  width: 120px;
  height: 29px;

  /* baslik3 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 130%;
  /* identical to box height, or 29px */

  text-align: center;

  /* Primary */

  color: #3c4e69;
  margin-bottom: 7px;
}
.giris {
  width: 177px;
  height: 47px;

  /* baslik1 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: 800;
  font-size: 36px;
  line-height: 130%;
  /* identical to box height, or 47px */

  text-align: center;
  letter-spacing: -0.01em;

  /* Secondary */

  color: white;
  margin-bottom: 35px;
}
/* .loginBox {
  width: auto;
  height: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
} */

.sifre {
  width: 468px;
  height: 60px;

  background: #ffffff;

  /* Form Shadow */

  box-shadow: 0px 3px 3px rgba(0, 0, 0, 0.03);
  border-radius: 6px;
  border: none;
  margin-bottom: 25px;

  /* form-baslik */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 100%;
  /* identical to box height, or 16px */

  letter-spacing: -0.01em;

  /* Gri */

  color: #818b9a;
  padding-left: 1rem;
}
.loginActions {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  /* border: 1px solid black; */
}
.hatirlaContainer {
  height: 21px;
  width: 100%;
  display: flex;
  flex-direction: row;
  /* justify-content: flex-start;
  align-items: flex-start; */
  margin-left: 1.2rem;
}
.unuttumContainer {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  align-items: center;
  /* border: 1px solid black; */
  margin-right: 1.2rem;
}
.hatirlaLogo {
  /* border: 1px solid black; */
  width: auto;
  height: auto;
  margin-right: 7px;
}
.unuttumLogo {
  width: auto;
  height: auto;
  /* border: 1px solid black; */
  text-align: right;
  /* border: 2px solid black; */
  justify-self: flex-end;
  margin-right: 7px;
}
.hatirlaPara {
  width: 100%;
  height: auto;
  /* border: 1px solid black; */

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
.unuttumPara {
  height: auto;
  width: auto;
  /* text3 */
  /* border: 2px solid black; */
  padding: 0;
  margin: 0;
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 15px;
  line-height: 140%;
  /* identical to box height, or 21px */

  letter-spacing: -0.01em;

  /* Primary */
  color: #3c4e69;
  text-align: right;
  justify-self: flex-end;
}
.loginBtn {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 12px 20px 11px;

  width: 484px;
  height: 50px;

  /* Turuncu */

  background: #ff8038;
  border-radius: 6px;
  border: none;

  /* buton-text-orta */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: 800;
  font-size: 16px;
  line-height: 110%;
  /* identical to box height, or 18px */

  display: flex;
  align-items: center;
  text-align: center;

  /* Beyaz */

  color: #ffffff;

  /* Inside auto layout */

  flex: none;
  order: 0;
  flex-grow: 0;
  margin: 0px 10px;

  margin-top: 19px;
}
.loginBox {
  width: auto;
  height: auto;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  /* border: 1px solid black; */
}
.inputs {
  width: 100%;
  /* border: 2px solid red; */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.inputCheck {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: flex-start;
}
.errorMsg {
  width: 239px;
  height: 16px;

  /* text05 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 12px;
  line-height: 130%;
  /* identical to box height, or 16px */

  /* Kirmizi */

  color: #ea5455;
  /* border: 1px solid black; */
}

.telBox {
  width: 100%;
  /* height: auto; */
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: flex-start;
  margin-bottom: 25px;
  /* border: 4px solid black; */
}
.countryCode {
  margin-right: 18px;
  width: 103px;
  height: 60px;

  background: #ffffff;
  /* Form Shadow */

  box-shadow: 0px 3px 3px rgba(0, 0, 0, 0.03);
  border-radius: 6px;
  border: none;
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 100%;
  /* identical to box height, or 16px */

  letter-spacing: -0.01em;

  /* Gri */

  color: #818b9a;
}
.telNo {
  width: 100%;
  height: 60px;

  background: #ffffff;
  /* Form Shadow */

  box-shadow: 0px 3px 3px rgba(0, 0, 0, 0.03);
  border-radius: 6px;
  border: none;
  /* form-baslik */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 100%;
  /* identical to box height, or 16px */

  letter-spacing: -0.01em;

  /* Gri */

  color: #818b9a;
}
</style>
