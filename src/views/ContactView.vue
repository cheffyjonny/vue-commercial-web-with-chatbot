<template>
  <div class="">
    <img
      class="mb-5"
      src="../assets/hero.jpg"
    />
    <div class="float-left text-left">
      <h1 class="text-3xl font-bold mb-3">Contact Us 🌹</h1>
      <Contacts />
    </div>
  </div>
</template>

<script>
/* eslint-disable */
import Hero from "@/components/Hero.vue";
import Feature from "@/components/Feature.vue";
import Contacts from "@/components/Contacts.vue";

export default {
  name: "ContactView",
  components: {
    Hero,
    Feature,
    Contacts,
  },
};
</script>
<style scoped>
img {
  border-radius: 20px;
  object-fit: cover;
  height: 12rem;
  overflow: hidden;
  width: 100%;
}
</style>
