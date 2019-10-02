<template>
  <div class="home">
    <AppHeader />
    <FoodPackages />
  </div>
</template>

<script>
// @ is an alias to /src
import AppHeader from "@/components/Header/AppHeader.vue";
import FoodPackages from "@/components/FoodPackages//FoodPackages";

export default {
  name: "home",
  components: {
    AppHeader,
    FoodPackages
  }
};
</script>
