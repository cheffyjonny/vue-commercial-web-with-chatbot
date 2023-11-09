<template>
  <div>
    <div class="flex mb-3">
      <h1 class="text-2xl font-bold">Featured Products 💐</h1>
    </div>
    <div class="grid grid-cols-2 items-center gap-2">
      <Card
        v-for="(card, index) in cards"
        :key="index"
        :src="card.src"
        :title="card.title"
        :price="card.price"
        :paragraph="card.paragraph"
      />
    </div>
  </div>
</template>
<script>
/* eslint-disable */
import Card from "@/components/Card.vue";
export default {
  name: "Feature",
  components: {
    Card,
  },
  data() {
    return {
      cards: [
        {
          src: require("../assets/a.jpg"),
          title: "Product A",
          price: "2.00",
          paragraph:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis expedita earum corrupti, dolorum dolores necessitatibus nihil laborum inventore dolore nesciunt.",
        },
        {
          src: require("../assets/b.jpg"),
          title: "Product B",
          price: "3.00",
          paragraph:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis expedita earum corrupti, dolorum dolores necessitatibus nihil laborum inventore dolore nesciunt.",
        },
        {
          src: require("../assets/c.jpg"),
          title: "Product C",
          price: "4.00",
          paragraph:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis expedita earum corrupti, dolorum dolores necessitatibus nihil laborum inventore dolore nesciunt.",
        },
        {
          src: require("../assets/d.jpg"),
          title: "Product D",
          price: "5.00",
          paragraph:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Reiciendis expedita earum corrupti, dolorum dolores necessitatibus nihil laborum inventore dolore nesciunt.",
        },
      ],
    };
  },
};
</script>
