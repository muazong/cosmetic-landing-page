<script setup lang="ts"></script>

<template>
  <section id="product-banner">
    <div class="product-banner-container">
      <div class="information">
        <h1>BỘT LÀM SÁNG DA VITABRID C12</h1>
        <p>
          Bí quyết dưỡng da trắng sáng, căng mịn, làm mờ thâm nám, đẩy lùi các dấu hiệu lão hoá.
        </p>

        <button class="buy-btn">
          <i class="pi pi-shopping-bag"></i>
          <p>ĐẶT MUA</p>
        </button>
      </div>

      <img src="@/assets/images/surprised-woman.png" alt="Surprised woman" />
    </div>
  </section>
</template>

<style scoped>
#product-banner {
  width: 100%;
  height: 64vh;
  padding: 0 40px;
  background: linear-gradient(45deg, #008c6c, #feb47b);
  display: flex;
  align-items: center;
  justify-content: center;
}

.product-banner-container {
  max-width: 1200px;
  display: flex;
  align-items: center;
  justify-content: space-evenly;

  img {
    height: 430px;
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

    .buy-btn {
      height: 50px;
      width: 120px;
      background-color: transparent;
      border: 2px solid #ffffff;
      border-radius: 12px;
      display: flex;
      align-items: center;
      justify-content: space-evenly;
      cursor: pointer;
      color: #ffffff;
      position: relative;

      &:hover {
        animation: shake 0.8s ease-in-out;
      }

      p {
        font-weight: bold;
      }
    }
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
