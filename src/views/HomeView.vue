<template>
  <div class="">
    <Hero />
    <Feature />
  </div>
</template>

<script>
import Hero from "@/components/Hero.vue";
import Feature from "@/components/Feature.vue";

export default {
  name: "HomeView",
  components: {
    Hero,
    Feature,
  },
};
</script>
