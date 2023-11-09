<template>
  <div class="w-1/2 pt-6 pb-14 flex flex-col">
    <h1
      class="text-6xl uppercase font-extrabold text-neutral-600 text-left mb-3"
    >
      WE SELL THE
      <span>FRESHEST</span>
      FLOWERS!
    </h1>
    <router-link to="/products">
      <CustomBtn
        class="self-start"
        :text="'BROWSE PRODUCTS'"
      />
    </router-link>
  </div>
</template>
<script>
/* eslint-disable */
import CustomBtn from "@/components/CustomBtn.vue";
export default {
  name: "Hero",
  components: {
    CustomBtn,
  },
};
</script>
<style scoped>
span {
  color: #e13985;
}
</style>
