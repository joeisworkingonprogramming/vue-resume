<template>
  <div class="page-wrapper">
    <div class="page" :id="$route.params.resumeid">
      <div class="page-inner">
        <component :is="$route.params.resumeid"></component>
      </div>
    </div>
  </div>
</template>

<script>
/* eslint-disable */
import Vue from "vue";
/* eslint-disable */
import "../resumes/resumes";
/* eslint-disable */
export default Vue.component("resume", {
  name: "app"
});
</script>

<style scoped>
.page-inner {
  height: 100%;
  width: 100%;
}
.page-wrapper {
  overflow-x: hidden;
  background: #cccccc;
  margin: 0;
  padding: 0;
  -webkit-print-color-adjust: exact;
  box-sizing: border-box;
}

.resume {
  height: 100%;
  width: 100%;
}

.page {
  background: white;
  position: relative;
  width: 21cm;
  /* height: 29.68cm; */
  display: block;
  page-break-after: auto;
  overflow: hidden;
  margin: 0 auto;
}
</style>
