<script>
import AppTitle from "./components/AppTitle.vue";
import AppBanner from "./components/AppBanner.vue";

export default {
  components: {
    AppTitle,
    AppBanner
  },
  data() {
    return {};
  },
};
</script>

<template>
  <h1>Hello</h1>

  <AppBanner />

  <section>
    <AppTitle />
  </section>
</template>

<style></style>
