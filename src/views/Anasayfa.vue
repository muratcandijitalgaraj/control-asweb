<template>
  <div class="anasayfa">
    <Header />
    <!-- <img src="../assets/anasayfa/bulutlar.svg" alt="" class="bulutlar" /> -->
    <div class="zemin">
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
  /* border: 6px solid black; */
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
  width: 65%;
  height: auto;

  background: #f2f8fb;
  box-shadow: 0px 4px 30px rgba(0, 0, 0, 0.15);
  border-radius: 18px;
  /* margin-bottom: 5px; */
  display: flex;
}
#sideBarLeft {
  width: auto;
}
#sideBarTop {
  display: none;
}
.rightPart {
  display: flex;
  flex-direction: column;
  /* border: 2px solid red; */
  width: auto;
}
.footerContainer {
  height: auto;
  width: 65%;
}
@media only screen and (max-width: 1500px) {
  #sideBarLeft {
    display: none;
  }
  #sideBarTop {
    display: block;
  }
  .zemin {
    height: auto;
    flex-direction: column;
  }
  .rightPart {
    display: flex;
    flex-direction: column;
  }
}
@media only screen and (max-width: 600px) {
  .zemin {
    width: 95%;
  }
}
</style>
