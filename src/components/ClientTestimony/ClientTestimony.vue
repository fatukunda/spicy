<template>
  <div class="container-fluid">
    <div class="row main">
      <div class="col-md-6">
        <div class="client-info">
          <h5 class="clients-say">
            <span class="clients">Clients</span>
            <span class="say">say</span>
          </h5>
          <div class="client-card">
            <h6 class="client-name">Frank Atukunda</h6>
            <p class="client-comment">
              It's a long established fact that a reader will be distracted by
              the readable content of a page when looking at it's layout. The
              point of using lorem Ipsum is that it has a more-or-less normal
              distribution of letters
            </p>
            <img :src="image" alt="quotes" class="quotes" />
            <img :src="avatar" alt="avatar" class="avatar" />
          </div>
        </div>
        <div class="dots">
          <img :src="dot" alt class="dot" />
          <img :src="whiteDot" alt class="dot" />
          <img :src="dot" alt class="dot" />
        </div>
      </div>
      <div class="col-md-6">
        <img :src="dish" alt="dish" class="dish-plate" />
      </div>
    </div>
  </div>
</template>

<script>
import quotes from "../../assets/left-quote.svg";
import avatar from "../../assets/avatar.png";
import food from "../../assets/dish.png";
import dot from "../../assets/dot.svg";
import whiteDot from "../../assets/dotwhite.svg";
export default {
  name: "ClientTestimony",
  data() {
    return {
      image: quotes,
      avatar,
      dish: food,
      dot,
      whiteDot
    };
  }
};
</script>

<style scoped>
.main {
  background: #5a2f27;
  height: 32rem;
}
.client-info {
  margin-left: 10rem;
}
.clients {
  color: #eda911;
  padding-right: 0.2rem;
}
.say {
  color: #ffffff;
}
.client-card {
  width: 25rem;
  height: 17rem;
  background-color: #ffffff;
  text-align: center;
  margin: 0 auto;
  margin-top: 6rem;
  position: relative;
}
.clients-say {
  margin-top: 4rem;
}
.client-comment {
  font-size: 12px;
  padding-right: 1rem;
  padding-left: 1rem;
  line-height: 1.5rem;
}
.client-name {
  color: #eda911;
  padding-top: 4rem;
}
.quotes {
  width: 2rem;
}
.avatar {
  width: 6rem;
  border-radius: 50%;
  position: absolute;
  top: -3rem;
  left: 9rem;
}
.dish-plate {
  width: 24rem;
  margin: 0 auto;
  margin-top: 11rem;
  margin-left: 10rem;
}
.dot {
  width: 1rem;
  padding: 0.2rem;
}
.dots {
  text-align: center;
  margin-left: 10rem;
  margin-top: 1rem;
}
@media screen and (max-width: 600px) {
  .client-info {
    margin-left: 0;
  }
  .client-card {
    width: 100%;
  }
  .avatar {
    left: 7rem;
  }
  .dish-plate {
    width: 100%;
    margin: 0 auto;
    margin-top: 4rem;
  }
  .dots {
    text-align: center;
    margin-left: 0;
  }
}
</style>
