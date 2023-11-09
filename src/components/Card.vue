<template>
  <div class="card">
    <img
      class="mb-5"
      :src="src"
    />
    <div class="flex flex-col items-start">
      <h1 class="font-extrabold mb-2">{{ title }}</h1>
      <h4 class="mb-2">${{ price }}</h4>
      <p class="text-left text-xs mb-3">{{ paragraph }}</p>
    </div>
    <CustomBtn
      class="w-full"
      :text="'ADD TO CART'"
    />
  </div>
</template>
<script>
/* eslint-disable */
import CustomBtn from "@/components/CustomBtn.vue";

export default {
  name: "Card",
  components: {
    CustomBtn,
  },
  props: {
    src: String,
    title: String,
    price: String,
    paragraph: String,
  },
};
</script>
<style scoped>
.card {
  background-color: #f5f5f5;
  border-radius: 15px;
  padding: 1rem;
}
img {
  border-radius: 20px;
  object-fit: cover;
  height: 8rem;
  overflow: hidden;
  width: 100%;
}
</style>
