<template>
  <div class="home">
    <button @click="decreaseCounter" class="btn">-</button>
    <span class="counter">{{ counter }}</span>
    <button @click="increaseCounter" class="btn">+</button>
  </div>
</template>

<script>
export default {
data() {
  return {
    counter: 0
  }
},
methods: {
  increaseCounter() {
    this.counter++;
  },
  decreaseCounter() {
    this.counter--;
  }
},
}
</script>


<style>
.home {
  text-align: center;
  padding: 20px;
}
.button .counter {
  font-size: 40px;
  padding: 10px;
}
</style>
