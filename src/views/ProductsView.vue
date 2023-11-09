<template>
  <div class="">
    <h1 class="text-left text-3xl font-extrabold mb-5">Products List 🌼</h1>
    <Lists />
  </div>
</template>

<script>
/* eslint-disable */
import Hero from "@/components/Hero.vue";
import Feature from "@/components/Feature.vue";
import Lists from "@/components/Lists.vue";

export default {
  name: "ProductsView",
  components: {
    Hero,
    Feature,
    Lists,
  },
};
</script>
