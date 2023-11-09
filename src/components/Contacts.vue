<template>
  <ul>
    <li
      v-for="(contact, index) in contacts"
      :key="index"
      class="ml-1 mb-2 font-semibold"
    >
      ✻ {{ capitalizeFirstLetter(contact.type) }} : {{ contact.info }}
    </li>
  </ul>
</template>

<script>
/* eslint-disable */

export default {
  name: "Contacts",
  data() {
    return {
      contacts: [
        {
          type: "address",
          info: "123 Blossom Street, Gardenia City, FL 54321",
        },
        { type: "phone", info: "(555) 123-4567" },
        { type: "email", info: "info@flowersrus.com" },
        { type: "website", info: "www.flowersrus.com" },
        {
          type: "facebook",
          info: "www.facebook.com/flowersrus",
        },
        {
          type: "instagram",
          info: "www.instagram.com/flowersrus",
        },
      ],
    };
  },
  methods: {
    capitalizeFirstLetter(string) {
      return string.charAt(0).toUpperCase() + string.slice(1);
    },
  },
};
</script>
