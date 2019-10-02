<template>
  <div class="container-fluid food-packages">
    <div class="row foods-container">
      <div class="col-md-12">
        <h5 class="text-center title">
          <span class="food">Food</span>
          <span class="packages">Packages</span>
        </h5>
        <p class="text-center description pt-2">
          There are many variations of passages of Lorem Ipsum available, but
          the majorityomised words which don't look even slightly believable
        </p>
      </div>
      <div class="col-md-12">
        <div class="row">
          <div class="col-md-4" v-for="dish in dishes" :key="dish.name">
            <Dish
              :avatar="dish.avatar"
              :name="dish.name"
              :description="dish.description"
              :color="dish.color"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Dish from "./Dish";
import macron from "../../assets/macrons.png";
import omlette from "../../assets/omlette.png";
import soup from "../../assets/soup.png";
export default {
  name: "FoodPackages",
  components: {
    Dish
  },
  data() {
    return {
      dishes: [
        {
          name: "Homemade",
          avatar: macron,
          description:
            "There are many variations of passages of Lorem Ipsum available, but the majorityomised words which don't look even slightly believable",
          color: "#5a2f27"
        },
        {
          name: "Noodles",
          avatar: soup,
          description:
            "There are many variations of passages of Lorem Ipsum available, but the majorityomised words which don't look even slightly believable",
          color: "#eda911"
        },
        {
          name: "Egg",
          avatar: omlette,
          description:
            "There are many variations of passages of Lorem Ipsum available, but the majorityomised words which don't look even slightly believable",
          color: "#5a2f27"
        }
      ]
    };
  }
};
</script>

<style scoped>
.food-packages {
  background: #fffbfb;
  height: 500px;
}
.food {
  color: #fdbe31;
  padding-right: 0.3rem;
}
.packages {
  color: #5a2f27;
}
.title {
  margin-top: 2rem;
  font-weight: bold;
}
.description {
  font-size: 12px;
}
.foods-container {
  width: 60%;
  margin: 0 auto;
}
@media screen and (max-width: 600px) {
  .foods-container {
    width: 100%;
  }
  .title {
    margin-top: 28rem;
  }
}
</style>
