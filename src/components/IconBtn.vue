<template>
  <button class="w-1/2 h-1/3">
    <i :class="'fa-solid fa-' + icon"></i>
  </button>
</template>
<script>
export default {
  name: "CustomBtn",
  props: {
    icon: String,
  },
};
</script>
<style scoped>
* {
  font-size: 0.8rem;
}
button {
  border-radius: 50px;
  padding-right: 10px;
  padding-left: 10px;
  padding-top: 5px;
  padding-bottom: 5px;
  font-weight: 600;
  color: #fff;
  background-color: #e13985;
}
</style>
