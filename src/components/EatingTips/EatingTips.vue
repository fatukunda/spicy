<template>
  <div class="container-fluid eating-tips">
    <div class="row intro">
      <div class="col-md-12">
        <small class="how-it-works">How it works</small>
        <h5 class="font-weight-bold pt-2">
          <span class="three-steps">3 Steps for</span>
          <span class="healthy-eating">Healthy Eating</span>
        </h5>
      </div>
      <div class="col-md-12">
        <div class="row tips">
          <div class="col-md-4 single-tip" v-for="tip in tips" :key="tip.id">
            <EatingTip
              :id="tip.id"
              :tip="tip.tip"
              :background="tip.background"
              :color="tip.color"
              :idColor="tip.idColor"
              :idBackgroundColor="tip.idBackgroundColor"
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import EatingTip from "./EatingTip";
export default {
  name: "EatingTips",
  components: {
    EatingTip
  },
  data() {
    return {
      tips: [
        {
          id: "01",
          tip:
            "available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable",
          background: "#FDBE31",
          color: "#ffffff",
          idBackgroundColor: "#5A2F27",
          idColor: "#ffffff"
        },
        {
          id: "02",
          tip:
            "available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable",
          background: "#EAE9E4",
          color: "##190707",
          idBackgroundColor: "#190707",
          idColor: "#ffffff"
        },
        {
          id: "03",
          tip:
            "available, but the majority have suffered alteration in some form, by injected humour, or randomised words which don't look even slightly believable",
          background: "#FDBE31",
          color: "#ffffff",
          idBackgroundColor: "#5A2F27",
          idColor: "#ffffff"
        }
      ]
    };
  }
};
</script>

<style scoped>
.eating-tips {
  margin-top: 6rem;
  margin-bottom: 4rem;
}
.intro {
  text-align: center;
  width: 60%;
  margin: 0 auto;
}
.three-steps {
  color: #fdbe31;
}
.healthy-eating {
  color: #5a2f27;
  padding-left: 0.3rem;
}
.how-it-works {
  color: #b3b1a6;
}
.tips {
  margin-top: 4rem;
}

@media screen and (max-width: 600px) {
  .intro {
    width: 100%;
    margin-top: 80rem;
  }
  .single-tip {
    margin-top: 0.5rem;
  }
}
</style>
