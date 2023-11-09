<template>
  <div>
    <span class="header flex">
      <h1
        v-for="(header, index) in headers"
        :key="index"
        :class="header.class"
      >
        {{ header.text }}
      </h1>
    </span>
    <List
      v-for="(card, index) in cards"
      :key="index"
      :src="card.src"
      :title="card.title"
      :price="card.price"
      :paragraph="card.paragraph"
    />
  </div>
</template>

<script>
/* eslint-disable */
import List from "@/components/List.vue";

export default {
  name: "Lists",
  components: {
    List,
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
      headers: [
        { class: "w-5/12", text: "Product Name" },
        { class: "w-2/12", text: "Price" },
        { class: "w-4/12", text: "Description" },
      ],
    };
  },
};
</script>
<style scoped>
.header {
  background-color: #f5f5f5;
  font-weight: 700;
  padding-top: 0.5rem;
  padding-bottom: 0.5rem;
  margin-bottom: 1rem;
  border-radius: 10px;
}
</style>
