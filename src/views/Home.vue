<template>
  <div class="home">
    <AppHeader />
    <FoodPackages />
    <EatingTips />
    <ClientTestimony />
    <AppAdvert />
    <AppFooter />
  </div>
</template>

<script>
// @ is an alias to /src
import AppHeader from "@/components/Header/AppHeader";
import FoodPackages from "@/components/FoodPackages//FoodPackages";
import EatingTips from "@/components/EatingTips/EatingTips";
import ClientTestimony from "@/components/ClientTestimony/ClientTestimony";
import AppAdvert from "@/components/AppAdvert/AddAdvert";
import AppFooter from "../components/Footer/AppFooter";

export default {
  name: "home",
  components: {
    AppHeader,
    FoodPackages,
    EatingTips,
    ClientTestimony,
    AppAdvert,
    AppFooter
  }
};
</script>
