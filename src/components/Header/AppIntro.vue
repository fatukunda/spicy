<template>
  <div class="col-md-12 intro">
    <h3 class="title">Healthy Food Recipes</h3>
    <p class="intro-text">
      There are many variations of passages of Lorem Ipsum available, but the
      majorityomised words which don't look even slightly believable
    </p>
    <button class="btn-readmore">Read More</button>
  </div>
</template>

<script>
export default {
  name: "AppIntro"
};
</script>

<style scoped>
.intro {
  margin-left: 10rem;
  margin-top: 4rem;
}
.title {
  width: 6rem;
  color: #5a2f27;
  font-size: 50px;
  font-weight: bold;
}
.intro-text {
  width: 20rem;
  font-size: 11px;
  color: #5a2f27;
  margin-top: 2rem;
}
.btn-readmore {
  color: #fcfbfa;
  background-color: #eda911;
  width: 8rem;
  height: 2.3rem;
  font-size: 15px;
  border: 0;
}
.btn-readmore:focus {
  outline: 0;
}

@media screen and (max-width: 600px) {
  .intro {
    margin-left: 0;
    margin-top: 2rem;
  }
}
</style>
