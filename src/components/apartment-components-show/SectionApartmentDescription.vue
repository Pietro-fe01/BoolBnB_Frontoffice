<template>
  <div class="row col-div">
    <div class="col-lg-7 col-xs-12 col-left">
      <ApartmentMainInfo :info="this.data" />
    </div>
    <div class="col-lg-5 col-xs-12 col-right">
        <PrenotationAside :info="this.data" />
    </div>
  </div>
</template>

<script>
import ApartmentMainInfo from "./ApartmentMainInfo.vue";
import PrenotationAside from "./PrenotationAside.vue";

export default {
  components: {
    ApartmentMainInfo,
    PrenotationAside,
  },
  props: {
    data: Object,
  },
};
</script>

<style lang="scss" scoped>
.row {
  margin-top: 1.25rem;
}

</style>
