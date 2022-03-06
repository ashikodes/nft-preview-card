<script setup>
import NFTCard from "./components/NFTCard.vue";
</script>

<template>
  <NFTCard />
  <div class="attribution">
    Challenge by&nbsp;
    <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">
      Frontend Mentor</a
    >.&nbsp;&nbsp;Coded by&nbsp;
    <a href="https://kodes.live">Kodes</a>
  </div>
</template>

<style>
@import "./assets/base.css";

#app {
  background-color: hsl(217, 54%, 11%);
  min-height: 100vh;
  font-family: "Outfit", sans-serif;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.attribution {
  font-size: 0.8rem;
  text-align: center;
  color: hsl(0, 0%, 100%);
  position: fixed;
  bottom: 1rem;
  width: 100%;
}
.attribution a {
  color: hsl(228, 45%, 44%);
}
</style>
