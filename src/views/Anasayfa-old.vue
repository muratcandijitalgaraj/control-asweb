<template>
  <div class="anasayfa">
    <Header />
    <!-- <img src="../assets/anasayfa/bulutlar.svg" alt="" class="bulutlar" /> -->
    <div class="zemin">
      <div class="zeminRow">
        <div id="sideBarLeft">
          <SideBarLeft />
        </div>
        <div id="sideBarTop">
          <SideBarTop />
        </div>
        <div class="rightPart">
          <Cards />
          <Randevularim />
        </div>
      </div>
      <div class="footerContainer">
        <Footer />
      </div>
    </div>
  </div>
</template>

<script>
import Header from "../components/anasayfa/Header.vue";
import SideBarLeft from "../components/anasayfa/SideBarLeft.vue";
import SideBarTop from "../components/anasayfa/SideBarTop.vue";
import Cards from "../components/anasayfa/Cards.vue";
import Randevularim from "../components/anasayfa/Randevularim.vue";
import Footer from "../components/Footer.vue";

export default {
  components: { Header, SideBarLeft, SideBarTop, Cards, Randevularim, Footer },
};
</script>

<style scoped>
.anasayfa {
  overflow-x: hidden;
  width: 100%;
  height: 100%;

  /* Secondary */

  background: #32a5df;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
  display: flex;
  flex-direction: column;
  margin: 0;
  padding: 0;
}

/* .bulutlar {
  margin-top: 10rem;
  position: absolute;

  height: auto;
  width: 100%;
} */
.zemin {
  margin-top: 27px;
  /* zemin */
  /* border: 2px solid red; */
  width: auto;
  height: 100%;

  background: #f2f8fb;
  box-shadow: 0px 4px 30px rgba(0, 0, 0, 0.15);
  border-radius: 18px;
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0;
  /* margin-bottom: 5px; */
  display: flex;
  flex-direction: column;
}
.zeminRow {
  /* margin-top: 27px; */
  /* zemin */
  width: auto;
  height: 100%;

  background: #f2f8fb;
  box-shadow: 0px 4px 30px rgba(0, 0, 0, 0.15);
  border-radius: 18px;
  border-bottom-left-radius: 0;
  border-bottom-right-radius: 0;
  /* margin-bottom: 5px; */
  display: flex;
}
#sideBarLeft {
  width: auto;
  height: 100%;
}
#sideBarTop {
  display: none;
}
.rightPart {
  display: flex;
  flex-direction: column;
  width: 100%;
}
.footerContainer {
  height: auto;
  width: auto;
  /* border: 2px solid black; */
}
/* @media only screen and (min-width: 1500px) {
  .zemin {
    width: 75%;
  }
} */
@media only screen and (max-width: 1250px) {
  #sideBarLeft {
    display: none;
  }
  #sideBarTop {
    display: block;
  }
  .zeminRow {
    width: auto;

    height: auto;
    flex-direction: column;
  }
  .rightPart {
    display: flex;
    flex-direction: column;
  }
}
@media only screen and (max-width: 750px) {
  .zeminRow {
    width: auto;
  }
  .footerContainer {
    width: auto;
  }
}
</style>
