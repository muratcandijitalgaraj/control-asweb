<template>
  <div class="middlePartComponent">
    <div class="container">
      <form class="welcomePart">
        <div class="hosgeldiniz">Hoşgeldiniz</div>
        <div class="giris">Giriş Yapın</div>
        <div class="telContainer">
          <input placeholder="+90" type="text" class="countryCode" />
          <div class="telefonNoContainer">
            <input placeholder="Telefon Numaranız" type="text" class="telNo" />
            <span v-bind:class="{ active: isActive }" class="errorMessage"
              >Geçerli bir telefon numarası yazın</span
            >
          </div>
        </div>
        <div class="sifreContainer">
          <input placeholder="Şifreniz" type="text" class="sifre" />
          <span v-bind:class="{ active: isActive }" class="errorMessage"
            >Hatalı şifre girdiniz</span
          >
        </div>
        <div class="loginActions">
          <div class="checkboxContainer">
            <div
              v-bind:class="{ checked: isChecked }"
              @click="handleCheck"
              class="unChecked"
            >
              <img
                src="../assets/giris/checkImg.svg"
                alt=""
                class="checkboxImg"
              />
            </div>
            <div @click="handleCheck" class="checkboxPara">Beni Hatırla</div>
          </div>
          <div class="forgotContainer">
            <img
              src="../assets/giris/flash-circle-1.svg"
              alt=""
              class="forgotLogo"
            />
            <div class="forgotPara">Şifremi Unuttum</div>
          </div>
        </div>
        <button @click="showError" class="tamamButton">Tamam</button>
      </form>
      <div class="bulutPart">
        <div class="orta-bulut">
          <!-- carousel will come here -->
          <!-- <img
            src="../assets/giris/imageGroup-1.svg"
            alt=""
            class="imageGroup"
          /> -->
          <Carousel />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Carousel from "./Carousel.vue";
export default {
  components: { Carousel },
  data() {
    return {
      isActive: false,
      isChecked: false,
    };
  },
  methods: {
    showError: function (e) {
      e.preventDefault();
      this.isActive = true;
    },
    handleCheck: function () {
      // e.preventDefault();
      this.isChecked = !this.isChecked;
      // console.log(this.isChecked);
    },
  },
};
</script>

<style scoped lang="scss">
//flex center mixin
@mixin flexCenter($direction) {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: $direction;
}
.middlePartComponent {
  width: 100%;
  height: 100%;
  // border: 1px solid red;
  @include flexCenter(row);
  margin-bottom: 50px;
}
.container {
  width: 65%;
  height: auto;
  // border: 1px solid red;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}
.welcomePart {
  // position: absolute;
  // left: 250px;
  // top: 250px;
  @include flexCenter(column);
  width: 468px;
  height: 100%;
  // border: 1px solid black;
  padding-top: 130px;
}
.hosgeldiniz {
  width: 121px;
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
  width: 178px;
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
  color: #32a5df;
  margin-bottom: 35px;
}
//there's nesting here
.telContainer {
  @include flexCenter(row);
  // margin-bottom: 25px;
  .telefonNoContainer {
    margin-bottom: 9px;
  }
}
.countryCode {
  width: 99.3px;
  height: 60px;
  background: #ffffff;
  /* Form Shadow */
  box-shadow: 0px 3px 3px rgba(0, 0, 0, 0.03);
  border-radius: 6px;
  border: none;
  margin-right: 18px;
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
  text-align: center;
  margin-bottom: 27px;
}
.telNo {
  width: 341px;
  height: 60px;
  background: #ffffff;
  /* Form Shadow */
  box-shadow: 0px 3px 3px rgba(0, 0, 0, 0.03);
  border-radius: 6px;
  border: none;
  /* Telefon Numaranız */
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

.sifre {
  width: 462px;
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
.loginActions {
  // border: 1px solid red;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  //took this part from w3schools
  //link=> https://www.w3schools.com/howto/howto_css_custom_checkbox.asp
}
.checkboxContainer {
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  align-items: center;
  // border: 2px solid black;
  width: auto;
  margin-left: 10px;
}
.unChecked {
  height: 20.166667938232422px;
  width: 20.166667938232422px;
  // border: 2px solid black;
  border-radius: 50%;
  background: white;
  margin-right: 7px;
}
.checked {
  background: #32a5df;
}
.checkboxPara {
  /* Beni Hatırla */
  width: 79px;
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
  // border: 2px solid black;
}
//forgot part starts
.forgotContainer {
  width: 100%;
  height: auto;
  // margin-top: 5px;
  margin-right: 10px;
  // border: 1px solid red;
  justify-content: flex-end;
  // border: 1px solid black;
  display: flex;
  flex-direction: row;
}
.forgotLogo {
  width: 22px;
  height: 22px;
  margin-right: 8.3px;
}
.forgotPara {
  width: auto;
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
  // border: 1px solid black;
}

//tamam button starts

.tamamButton {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  padding: 12px 20px 11px;
  width: 468px;
  height: 50px;
  /* Turuncu */
  background: #ff8038;
  border-radius: 6px;
  /* buton-text-orta */
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: 800;
  font-size: 16px;
  line-height: 110%;
  color: white;
  border: none;
}
.errorMessage {
  // border: 1px solid red;
  // change opacity to 0% to hide the element without changing the layout
  opacity: 0;
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
  margin-left: 10px;
}
.active {
  opacity: 1;
}
//bulut part starts here
.bulutPart {
  // @include flexCenter(column);
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  align-items: center;
  margin-top: 42px;
  // border: 1px solid black;
  width: 800px;
  height: 600px;
  // border: 1px solid red;
}
.orta-bulut {
  width: 585px;
  height: 211px;
  // border: 1px solid gold;
  background: url("../assets/giris/orta-bulut.svg");
  // background: black;
  @include flexCenter(column);
}
.imageGroup {
  width: auto;
  height: auto;
  overflow: visible;
  padding-top: 30rem;
  // margin-bottom: 50px;
}
// tablet starts here
@media only screen and (max-width: 1200px) {
  .container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .bulutPart {
    width: 100vw;
    // height: auto;
    // border: 1px solid gold;
    background: #e9f3f9;
    // padding-top: 30rem;
    pointer-events: none;
  }
  .orta-bulut {
    // border: 1px solid black;
  }
  .welcomePart {
    padding-top: 3rem;
  }
}
@media only screen and (max-width: 550px) {
  .welcomePart {
    // padding-top: 3rem;
    width: 100%;
  }
  .loginActions {
    @include flexCenter(column);
    width: 100%;
  }
  .checkboxContainer {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    align-items: center;
    width: 170px;
    margin: 0 0 5px 3.5px;
  }
  .unChecked {
    height: 20.166667938232422px;
    width: 20.166667938232422px;
    // border: 2px solid black;
    border-radius: 50%;
    background: white;
    margin-right: 7px;
  }
  .checked {
    background: #32a5df;
  }
  .checkboxPara {
    /* Beni Hatırla */
    width: 79px;
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
  .forgotContainer {
    width: 170px;
    display: flex;
    justify-content: flex-start;
    margin: 0;
  }
  .forgotPara {
    width: auto;
  }
  .telContainer {
    // border: 1px solid black;
    width: auto;
  }
  .countryCode {
    width: 100px;
  }
  .telefonNoContainer {
    // border: 1px solid black;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    width: auto;
  }
  .telNo {
    width: 100%;
  }
  .sifreContainer {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    width: 100%;
  }
  .sifre {
    width: 100%;
  }
  .tamamButton {
    width: 100%;
  }
}
</style>
