<template>
  <ul>
    <NavItem v-for="item in items" :key="item" :name="item" />
  </ul>
</template>

<script>
import NavItem from "./NavItem";
export default {
  name: "NavItems",
  data() {
    return {
      items: ["About", "Screenshot", "Contact"]
    };
  },
  components: {
    NavItem
  }
};
</script>

<style scoped></style>
