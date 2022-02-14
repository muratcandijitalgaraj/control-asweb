<template>
  <div class="muayeneler">
    <MuayeneCell />
  </div>
</template>

<script>
import MuayeneCell from "../anasayfa/MuayeneCell.vue";

export default { components: { MuayeneCell } };
</script>

<style scoped>
.muayeneler {
  height: auto;
  /* margin-left: 1rem; */
}
</style>
