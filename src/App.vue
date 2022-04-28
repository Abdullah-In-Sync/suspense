<template>
  <suspense>
    <Loader />
    <template #fallback>
      Loading...
    </template>
  </suspense>
</template>

<script>
import Loader from "./components/Loader.vue";

export default {
  name: "App",
  components: {
    Loader,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
