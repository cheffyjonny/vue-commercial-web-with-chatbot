<template>
  <CustomNav />
  <router-view />
</template>

<script>
import CustomNav from "@/components/CustomNav.vue";

export default {
  name: "HomeView",
  components: {
    CustomNav,
  },
};
</script>
<style>
body {
  background-color: #e7e5e4;
}
#app {
  font-family: ui-sans-serif, system-ui, -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", sans-serif,
    "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-left: auto;
  margin-right: auto;
  padding-left: 1rem;
  padding-right: 1rem;
  max-width: 56rem;
  padding-bottom: 3rem;
}

nav {
  padding-top: 30px;
  padding-bottom: 30px;
}

nav a {
  font-weight: bold;
  color: #000;
  opacity: 0.3;
}

nav a.router-link-exact-active {
  color: #000;
  opacity: 1;
}
</style>
