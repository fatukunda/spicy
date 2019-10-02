<template>
  <div class="home">
    <AppHeader />
  </div>
</template>

<script>
// @ is an alias to /src
import AppHeader from "@/components/Header/AppHeader.vue";

export default {
  name: "home",
  components: {
    AppHeader
  }
};
</script>
