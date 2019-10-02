<template>
  <div class="dish-container">
    <div class="dish" :style="{ backgroundColor: color }">
      <h6 class="text-center font-weight-bold">{{ name }}</h6>
      <p class="text-center">{{ description }}</p>
    </div>
    <img :src="avatar" :alt="name" class="avatar" />
  </div>
</template>

<script>
export default {
  name: "Dish",
  props: ["name", "avatar", "description", "color"]
};
</script>

<style scoped>
.dish-container {
  width: 15rem;
  height: 12rem;
  margin: 0 auto;
  position: relative;
}
.avatar {
  position: absolute;
  top: -7rem;
  right: 0.7rem;
}
.dish {
  color: #ffffff;
  font-size: 11px;
  height: 15rem;
  margin-top: 10rem;
  padding-top: 7rem;
  width: 16rem;
  line-height: 1.3rem;
}

@media screen and (max-width: 600px) {
  .dish-container {
    width: 100%;
    height: 12rem;
    margin: 0 auto;
    position: relative;
  }
  .dish {
    height: 15rem;
    margin-top: 11rem;
    width: 100%;
    line-height: 1.5rem;
  }
  .avatar {
    right: 2.5rem;
  }
}
</style>
