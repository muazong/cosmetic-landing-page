<script setup lang="ts">
import BuyButton from './Deltail/components/BuyButton.vue'
</script>

<template>
  <div id="home" class="component-container home-container">
    <section class="home section">
      <div class="home-product-info">
        <h2 class="sub-title">BỘT LÀM SÁNG DA</h2>
        <h1 class="main-title">VITABRID C12</h1>

        <p class="text">
          Công nghệ lớp khoáng kép LDH độc quyền của Huyndai Bioscience kết hợp với Vitamin C và
          nhiều loại dưỡng chất. Giúp dưỡng da trắng sáng, căng mịn, làm mờ thâm nám, đẩy lùi các
          dấu hiệu lão hoá.
        </p>

        <BuyButton />
      </div>

      <img class="home-product-img" src="@/assets/images/banner-1.png" alt="Vitabrid c12" />
    </section>

    <div class="scroll-mouse">
      <img src="@/assets/gifs/scrolling_mousewheel-1.gif" alt="mouse scrolling" />
    </div>
  </div>
</template>

<style scoped>
.home-container {
  height: auto;
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;

  overflow: hidden;
  background: linear-gradient(45deg, #008c6c, #feb47b);
  position: relative;
}

.home {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 0 40px;

  .home-product-info {
    color: #ffffff;
    max-width: 550px;
    display: flex;
    flex-direction: column;
    align-items: flex-start;

    .main-title {
      font-size: 4rem;
      margin: 20px 0;
    }
    .sub-title {
      font-size: 2.5rem;
    }
    .text {
      text-align: justify;
      font-size: 14px;
      line-height: 1.5;
    }

    .buy-btn {
      display: flex;
      align-items: center;
      justify-content: space-evenly;

      margin-top: 20px;
      background-color: transparent;
      border-radius: 12px;
      border: 2px solid #ffffff;
      color: #ffffff;
      height: 50px;
      position: relative;
      width: 120px;

      &:hover {
        animation: shake 0.8s ease-in-out;
        cursor: pointer;
      }

      p {
        font-weight: bold;
      }
    }
  }

  .home-product-img {
    height: 600px;
    margin-top: 100px;
    margin-right: -100px;
  }
}

.scroll-mouse {
  position: absolute;
  bottom: 30px;

  img {
    height: 56px;
    width: 44px;
  }
}

@media (max-width: 768px) {
  .home {
    flex-direction: column-reverse;

    .home-product-info {
      align-items: center;

      .main-title {
        font-size: 2rem;
        margin: 16px 0;
      }
      .sub-title {
        font-size: 1rem;
      }
      .text {
        text-align: center;
        font-size: 15px;
        line-height: 1.5;
      }
    }

    .home-product-img {
      margin-top: 20px;
      height: 300px;
      margin-right: unset;
    }
  }

  .scroll-mouse {
    display: none;
  }
}

@media (min-width: 768px) and (max-width: 1024px) {
  .home {
    .home-product-info {
      align-items: center;

      .main-title {
        font-size: 2rem;
        margin: 20px 0;
      }
      .sub-title {
        font-size: 1.5rem;
      }
      .text {
        text-align: center;
      }
    }
  }

  .scroll-mouse {
    display: none;
  }
}

@media (min-width: 1024px) {
}
</style>
