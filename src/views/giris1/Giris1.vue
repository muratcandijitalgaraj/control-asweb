<template>
  <div class="mainComponent">
    <div class="desktop">
      <Desktop />
    </div>
    <div class="tablet">
      <Tablet />
    </div>
  </div>
</template>

<script>
import Desktop from "./Desktop.vue";
import Tablet from "./Tablet.vue";
export default {
  components: { Desktop, Tablet },
};
</script>

<style scoped>
/* hide a view on a certain width */
/* hide desktop when it gets smaller */
@media only screen and (max-width: 1190px) {
  .desktop {
    display: none;
  }
}
/* hide tablet on desktop */
@media only screen and (min-width: 1191px) {
  .tablet {
    display: none;
  }
}
/* show tablet */
@media only screen and (max-width: 1190px) {
  .tablet {
    width: auto;
    height: 100%;
    /* background: black; */
  }
}
</style>
