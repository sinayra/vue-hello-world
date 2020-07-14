<template>
  <div v-lazy-container="{ selector: 'img' }">
    <img v-bind:data-src="data" />
    <span v-for="index in 10" :key="index"><br /></span>
  </div>
</template>

<script>
import Vue from "vue";
import VueLazyload from "vue-lazyload";

Vue.use(VueLazyload, {
  preLoad: 1.3,
  error: "./error.png",
  loading: "./loading.gif",
  attempt: 1,
});

export default {
  name: "LazyImage",
  props: ["data"],
};
</script>

<style scoped></style>
