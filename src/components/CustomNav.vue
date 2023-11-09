<template>
  <nav class="flex justify-between">
    <div
      @click="$router.push('/')"
      class="text-2xl font-black cursor-pointer"
    >
      Flowers`R`Us 🌷
    </div>
    <div class="w-1/3 flex justify-around item-center text-center">
      <router-link to="/">Home</router-link>
      <router-link to="/products">Products</router-link>
      <router-link to="/contact">Contact</router-link>
      <CustomBtn :text="'CART(0)'" />
    </div>
  </nav>
</template>
<script>
import CustomBtn from "./CustomBtn.vue";
export default {
  components: {
    CustomBtn,
  },
};
</script>
<style>
a {
  display: flex;
  align-items: center;
}
</style>
