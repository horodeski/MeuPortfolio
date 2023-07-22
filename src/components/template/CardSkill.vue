<script setup>
defineProps({
  description: String,
});
</script>

<template>
  <div class="card">
    <div class="top">
      <div class="dots">
        <div class="dot dot-1"></div>
        <div class="dot dot-2"></div>
        <div class="dot dot-3"></div>
      </div>
    </div>
    <div class="bottom">
      <p class="code">
        {{ description }}
      </p>
    </div>
  </div>
</template>

<style scoped>
.card {
  margin: 40px 0;
  width: 31%;
  height: 30vh;
  background: #111;
  border: 2px solid #000;
  border-radius: 5px;
}

.top {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin: 10px;
}

.dots {
  display: flex;
  gap:7px;
}

.dot {
  width: 15px;
  height: 15px;
  border-radius: 50%;
}

.dot-1 {
  background-color: rgb(0, 132, 255);
}

.dot-2 {
  background-color: rgb(39, 64, 94);
}

.dot-3 {
  background-color: rgb(0, 66, 75);
}



.bottom {
  margin-top: 30px;
  padding: 0 25px;
}

.code {
  font-size: 15px;
}
</style>
