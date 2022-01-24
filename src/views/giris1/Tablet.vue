<template>
  <div class="tabletComponent">
    <div class="bulutlar">
      <Header />
      <MiddlePart />
      <img src="../../assets/giris/sol-bulut.svg" alt="" class="sol-bulut" />
      <img src="../../assets/giris/sag-bulut.svg" alt="" class="sag-bulut" />
    </div>
    <BottomPart />
    <Footer />
  </div>
</template>

<script>
import Header from "../../components/giris/tablet/Header.vue";
import MiddlePart from "../../components/giris/tablet/MiddlePart.vue";
import BottomPart from "../../components/giris/tablet/BottomPart.vue";
import Footer from "../../components/giris/tablet/Footer.vue";

export default {
  components: { Header, MiddlePart, BottomPart, Footer },
};
</script>

<style scoped>
.tabletComponent {
  width: 100%;
  height: 100%;
  background: #e9f3f9;
}
.bulutlar {
  width: 100%;
  height: auto;
  left: 0px;
  top: 0px;

  background: linear-gradient(
      180deg,
      #33a5df 16.85%,
      rgba(51, 165, 223, 0) 58.86%
    ),
    linear-gradient(0deg, #e9f3f9 12.23%, rgba(233, 243, 249, 0) 77.17%),
    url("../../assets/giris/bulutlar.png");
  background-repeat: no-repeat;
}
.sol-bulut {
  position: absolute;
  width: 507px;
  height: 183px;
  left: -11rem;
  top: 83px;

  /* transform: matrix(-1, 0, 0, 1, 0, 0); */
}
.sag-bulut {
  position: absolute;
  width: 507px;
  height: 183px;
  /* left: 2239px; */
  right: -10rem;
  top: 51px;

  /* transform: matrix(-1, 0, 0, 1, 0, 0); */
}
</style>
