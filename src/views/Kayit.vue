<template>
  <div class="forBackgroundColor">
    <div class="kayitComponent">
      <Header para="Üye misiniz?" buttonText="Giriş Yap" />
      <Bulutlar />
      <MainPart />
      <Bottom />
      <Footer />
    </div>
  </div>
</template>

<script>
import Header from "../components/Header.vue";
import Bulutlar from "../components/kayit1/Bulutlar.vue";
import MainPart from "../components/kayit1/MainPart.vue";
import Bottom from "../components/Bottom.vue";
import Footer from "../components/Footer.vue";

export default {
  components: { Header, Bulutlar, MainPart, Bottom, Footer },
};
</script>

<style scoped lang="scss">
$backgroundColor: #e9f3f9;
.forBackgroundColor {
  width: 100%;
  height: 100%;
  background: $backgroundColor;
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}
.kayitComponent {
  width: 100%;
  //will change this later on
  height: 500px;
  background: linear-gradient(
      0deg,
      #e9f3f9 12.23%,
      rgba(233, 243, 249, 0) 77.17%
    ),
    url("../assets/giris/bulutlar.svg");
  background-repeat: no-repeat;
}
</style>
