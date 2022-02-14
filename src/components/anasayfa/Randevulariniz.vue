<template>
  <div class="randevulariniz">
    <Cell />
    <TallCell />
    <GreenCell />
  </div>
</template>

<script>
import Cell from "../anasayfa/Cell.vue";
import TallCell from "../anasayfa/TallCell.vue";
import GreenCell from "../anasayfa/GreenCell.vue";

export default { components: { Cell, TallCell, GreenCell } };
</script>

<style scoped>
.randevulariniz {
  height: auto;
  /* margin-left: 1rem; */
}
</style>
