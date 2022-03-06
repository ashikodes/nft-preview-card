<script setup>
import EthereumIcon from "./icons/icon-ethereum.vue";
import ClockIcon from "./icons/icon-clock.vue";
import ViewIcon from "./icons/icon-view.vue";
</script>

<template>
  <div class="card">
    <div class="img-wrapper">
      <div class="view-highlight">
        <ViewIcon />
      </div>
    </div>
    <h1>Equilibrium #3429</h1>
    <p>Our Equilibrium collection promotes balance and calm.</p>
    <div class="price-date">
      <span class="price"><EthereumIcon />0.041 ETH</span>
      <span class="date"><ClockIcon />3 days left</span>
    </div>
    <div class="author">
      <img src="src/assets/images/image-avatar.png" alt="author" />
      Creation of&nbsp;<span class="author-name">Jules Wyvern</span>
    </div>
  </div>
</template>

<style scoped>
.card {
  background-color: hsl(216, 50%, 16%);
  border-radius: 0.75rem;
  padding: 1.5rem;
  width: 90%;
}
.card .img-wrapper {
  background-image: url("src/assets/images/image-equilibrium.jpg");
  height: 300px;
  background-size: cover;
  border-radius: 0.75rem;
  width: 100%;
  cursor: pointer;
}
.card .view-highlight {
  border-radius: 0.75rem;
  width: 100%;
  height: 100%;
  display: none;
  align-items: center;
  justify-content: center;
}
.card .img-wrapper:hover .view-highlight {
  display: flex;
  background-color: hsla(178, 100%, 50%, 50%);
}
.card h1 {
  color: hsl(0, 0%, 100%);
  font-size: 1.5rem;
  margin-top: 1rem;
  cursor: pointer;
}
.card h1:hover {
  color: hsl(178, 100%, 50%);
}
.card p {
  color: hsl(215, 51%, 70%);
  margin: 1rem 0;
  font-size: 1.125rem;
}
.card .price-date {
  display: flex;
  justify-content: space-between;
}
.price-date span {
  display: flex;
  align-items: center;
}
.price-date svg {
  margin-right: 0.5rem;
}
.price-date .price {
  color: hsl(178, 100%, 50%);
}
.price-date .date {
  color: hsl(215, 51%, 70%);
}
.author {
  color: hsl(215, 51%, 70%);
  font-size: 1rem;
  display: flex;
  padding: 0.75rem 0 0.25rem;
  align-items: center;
  border-top: 1px solid hsl(215, 32%, 27%);
  margin-top: 1.25rem;
}
.author img {
  width: 30px;
  border: 1px solid hsl(0, 0%, 100%);
  border-radius: 50%;
  margin-right: 1rem;
}
.author .author-name {
  color: hsl(0, 0%, 100%);
  cursor: pointer;
}
.author .author-name:hover {
  color: hsl(178, 100%, 50%);
}
@media (min-width: 425px) {
  .card {
    width: 360px;
  }
}
</style>
