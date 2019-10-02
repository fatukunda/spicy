<template>
  <div
    class="eating-tip"
    :style="{ backgroundColor: background, color: color }"
  >
    <div
      class="tip"
      :style="{ backgroundColor: idBackgroundColor, color: idColor }"
    >
      <h5 class="text-center">{{ id }}</h5>
    </div>
    <p class="tip-description">{{ tip }}</p>
  </div>
</template>

<script>
export default {
  name: "EatingTip",
  props: ["id", "tip", "color", "background", "idColor", "idBackgroundColor"]
};
</script>

<style>
.tip {
  width: 5rem;
  height: 5rem;
  border-radius: 50%;
  position: absolute;
  top: -2rem;
  left: -1rem;
}
.tip h5 {
  line-height: 5rem;
}
.eating-tip {
  position: relative;
  height: 13rem;
  border-radius: 0 2rem 0 2rem;
}
.tip-description {
  font-size: 12px;
  line-height: 1.5rem;
  padding-top: 4rem;
}
</style>
