<template>
  <TheHeader title="RememberMe" />
  <TheResource />
</template>

<script>
import TheHeader from "./layout/TheHeader.vue";
import TheResource from "./components/learning-resource/TheResource.vue";
export default {
  name: "App",
  components: {
    TheHeader,
    TheResource,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
</style>
