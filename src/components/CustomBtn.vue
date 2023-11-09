<template>
  <button>
    {{ text }}
    {{ icon }}
  </button>
</template>
<script>
export default {
  name: "CustomBtn",
  props: {
    text: String,
    icon: String,
  },
};
</script>
<style scoped>
* {
  font-size: 0.8rem;
}
button {
  border-radius: 10px;
  padding-right: 10px;
  padding-left: 10px;
  padding-top: 5px;
  padding-bottom: 5px;
  font-weight: 600;
  color: #fff;
  background-color: #e13985;
}
</style>
