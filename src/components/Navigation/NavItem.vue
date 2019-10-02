<template>
  <router-link class="nav-item" to="url">{{ name }}</router-link>
</template>

<script>
export default {
  name: "NavItem",
  props: ["name", "url"]
};
</script>

<style scoped>
.nav-item {
  color: #eda911;
  padding: 1rem;
  text-transform: uppercase;
  font-size: 13px;
}
</style>
