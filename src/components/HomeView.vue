<script setup lang="ts"></script>

<template>
  <section id="home">
    <div class="home-container">
      <div class="information">
        <h2>BỘT LÀM SÁNG DA</h2>
        <h1>VITABRID C12</h1>
        <p>
          Công nghệ lớp khoáng kép LDH độc quyền của Huyndai Bioscience kết hợp với Vitamin C và
          nhiều loại dưỡng chất. Giúp dưỡng da trắng sáng, căng mịn, làm mờ thâm nám, đẩy lùi các
          dấu hiệu lão hoá.
        </p>

        <button class="buy-btn">
          <i class="pi pi-shopping-bag"></i>
          <p>ĐẶT MUA</p>
        </button>
      </div>
      <img class="banner" src="@/assets/images/banner-1.png" alt="banner" />
    </div>

    <div class="scroll-mouse">
      <img src="@/assets/gifs/scrolling_mousewheel-1.gif" alt="mouse scrolling" />
    </div>
  </section>
</template>

<style scoped>
#home {
  height: 100vh;
  width: 100%;
  background: linear-gradient(45deg, #008c6c, #feb47b);
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  overflow: hidden;
  padding: 120px;
  position: relative;
}

.home-container {
  margin-top: 180px;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: space-evenly;
  position: relative;
}

.information {
  color: #ffffff;
  max-width: 550px;

  & > * {
    margin: 20px 0;
  }

  h1 {
    font-size: 4rem;
  }

  h2 {
    font-size: 2.5rem;
  }

  p {
    text-align: justify;
    font-size: 14px;
    line-height: 1.5;
  }
}

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

.banner {
  width: 100%;
}

.scroll-mouse {
  display: absolute;
  bottom: 0;

  img {
    height: 56px;
    width: 44px;
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
