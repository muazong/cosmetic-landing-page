<script setup lang="ts">
import BuyButton from './BuyButton.vue'
</script>

<template>
  <div class="product-banner-container detail-component">
    <section class="section product-banner">
      <div class="information">
        <h1 class="title">BỘT LÀM SÁNG DA VITABRID C12</h1>
        <p class="subtitle">
          Bí quyết dưỡng da trắng sáng, căng mịn, làm mờ thâm nám, đẩy lùi các dấu hiệu lão hoá.
        </p>

        <BuyButton />
      </div>

      <img src="@/assets/images/surprised-woman.png" alt="Surprised woman" />
    </section>
  </div>
</template>

<style scoped>
.product-banner-container {
  background: linear-gradient(45deg, #008c6c, #feb47b);
  display: flex;
  align-items: center;
  justify-content: center;
}

.product-banner {
  display: flex;
  align-items: center;
  justify-content: space-evenly;

  img {
    height: 430px;
    margin-top: -80px;
  }

  .information {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    max-width: 600px;
    text-align: center;
    gap: 20px;
    color: #fff;
  }
}

@media (max-width: 768px) {
  .product-banner {
    img {
      display: none;
    }
  }
}

@media (min-width: 768px) and (max-width: 1024px) {
  .product-banner {
    img {
      height: 300px;
    }
  }
}
</style>
