<template>
  <div class="randevularim">
    <div class="texts">
      <div class="title">Randevularınız</div>
      <div class="showAll">Hepsini Göster</div>
    </div>
    <Cell />
    <TallCell />
    <Cell />
    <div class="texts">
      <div class="title">Son Muayeneler</div>
      <div class="showAll">Hepsini Göster</div>
    </div>
    <MuayeneCell />
  </div>
</template>

<script>
import Cell from "./RandevuCell.vue";
import TallCell from "./TallCell.vue";
import MuayeneCell from "./MuayeneCell.vue";

export default { components: { Cell, TallCell, MuayeneCell } };
</script>

<style scoped>
.randevularim {
  width: auto;
  height: 100%;

  /* border: 2px solid red; */
}
.randevularim * {
  margin-bottom: 20px;
}
.texts {
  /* border: 1px solid black; */
  height: auto;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding-left: 30px;
  padding-right: 30px;
  padding-bottom: 0;
  margin-bottom: 0;
}
.title {
  width: auto;
  height: 29px;

  /* baslik3 */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 22px;
  line-height: 130%;
  /* identical to box height, or 29px */

  /* Secondary */

  color: #32a5df;
}
.showAll {
  width: auto;
  height: 17px;

  /* text4-bold */

  font-family: Nunito Sans;
  font-style: normal;
  font-weight: bold;
  font-size: 13px;
  line-height: 130%;
  /* identical to box height, or 17px */

  letter-spacing: -0.01em;

  /* Gri */

  color: #818b9a;
}
</style>
