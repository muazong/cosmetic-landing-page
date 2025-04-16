<script setup lang="ts">
defineProps<{
  text?: string
}>()
</script>

<template>
  <button class="buy-btn">
    <i class="pi pi-shopping-bag"></i>
    <p>{{ text ? text : 'ĐẶT MUA' }}</p>
  </button>
</template>

<style>
.buy-btn {
  height: 50px;
  min-width: 120px;
  padding: 4px 8px;
  background-color: transparent;
  border: 2px solid #ffffff;
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  cursor: pointer;
  color: #ffffff;
  position: relative;
  gap: 4px;

  &:hover {
    animation: shake 0.8s ease-in-out;
  }

  p {
    font-weight: bold;
  }
}

@keyframes shake {
  0% {
    transform: translateX(0);
  }
  20% {
    transform: translateX(-7px);
  }
  40% {
    transform: translateX(7px);
  }
  60% {
    transform: translateX(-7px);
  }
  80% {
    transform: translateX(7px);
  }
  100% {
    transform: translateX(0);
  }
}
</style>
