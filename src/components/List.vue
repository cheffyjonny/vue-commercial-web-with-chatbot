<template>
  <div class="list">
    <div class="flex flex-col w-5/12">
      <img
        class="w-full h-full"
        :src="src"
      />
      <p class="font-medium">{{ title }}</p>
    </div>

    <h4 class="mb-2 w-2/12">${{ price }}</h4>
    <p class="w-4/12 text-left text-xs mb-3">{{ paragraph }}</p>

    <div class="flex items-center justify-center w-1/12">
      <IconBtn :icon="'basket-shopping'" />
    </div>
  </div>
</template>
<script>
/* eslint-disable */
import IconBtn from "@/components/IconBtn.vue";

export default {
  name: "Card",
  components: {
    IconBtn,
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
.list {
  background-color: #f5f5f5;
  border-radius: 15px;
  padding: 0.7rem;
  display: flex;
  margin-bottom: 1rem;
  height: 8rem;
}
img {
  border-radius: 20px;
  object-fit: cover;
  height: 100%;
  overflow: hidden;
}
</style>
