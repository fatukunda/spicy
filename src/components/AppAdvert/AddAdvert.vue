<template>
  <div class="container main">
    <div class="row main-info">
      <div class="col-md-12 text-center">
        <h5>Free Multipurpose</h5>
        <h5>Responsive Landing Page 2019</h5>
        <p class="light-yellow">
          <small>Modern lighting fast & easily customizable</small>
        </p>
        <button class="mt-4 quote-button">Get a quote</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppAdvert"
};
</script>

<style scoped>
.main {
  height: 20rem;
}
.main-info {
  margin-top: 6rem;
}
.light-yellow {
  color: #eda911;
  font-size: 0.8rem;
}
.quote-button {
  background-color: #eda911;
  width: 10rem;
  height: 2rem;
  border: 0;
  border-radius: 4rem;
  color: #ffffff;
  font-size: 0.8rem;
}
@media screen and (max-width: 600px) {
  .main-info {
    margin-top: 22rem;
  }
  .main {
    height: 15rem;
  }
}
</style>
