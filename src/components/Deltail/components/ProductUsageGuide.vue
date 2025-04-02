<script setup lang="ts"></script>

<template>
  <section id="product-usage-guide">
    <h1>HƯỚNG DẪN SỬ DỤNG</h1>
    <div class="product-usage-guide">
      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Labore, ab!</p>

      <div class="guide-steps">
        <div class="step">
          <img src="@/assets/images/guide.png" alt="step" />
          <h3 class="step-text">BƯỚC 1</h3>
          <p class="step-detail">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus quas, delectus
            deserunt cum laudantium neque.
          </p>
        </div>
        <div class="step">
          <img src="@/assets/images/guide.png" alt="step" />
          <h3 class="step-text">BƯỚC 2</h3>
          <p class="step-detail">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus quas, delectus
            deserunt cum laudantium neque.
          </p>
        </div>
        <div class="step">
          <img src="@/assets/images/guide.png" alt="step" />
          <h3 class="step-text">BƯỚC 3</h3>
          <p class="step-detail">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus quas, delectus
            deserunt cum laudantium neque.
          </p>
        </div>
        <div class="step">
          <img src="@/assets/images/guide.png" alt="step" />
          <h3 class="step-text">BƯỚC 4</h3>
          <p class="step-detail">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatibus quas, delectus
            deserunt cum laudantium neque.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
#product-usage-guide {
  height: 76vh;
  width: 100%;
  padding: 0 40px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 2rem;

  h1 {
    font-size: 2rem;
  }
}

.product-usage-guide {
  max-width: 1100px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 2rem;

  p {
    font-size: 14px;
    color: rgba(0, 0, 0, 0.8);
  }

  .guide-steps {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 12px;

    .step {
      gap: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      text-align: center;

      .step-detail {
        font-size: 13px;
        color: rgba(0, 0, 0, 0.8);
        line-height: 1.5;
        word-break: break-word;
        word-wrap: break-word;
      }
    }
  }
}
</style>
