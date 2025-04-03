<script setup lang="ts"></script>

<template>
  <div class="component-container product-usage-guide-container detail-component">
    <h1 class="title">HƯỚNG DẪN SỬ DỤNG</h1>

    <section class="section product-usage-guide">
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
    </section>
  </div>
</template>

<style scoped>
.product-usage-guide-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  gap: 1rem;
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
    text-align: center;
  }

  .guide-steps {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    max-width: 1200px;
    gap: 18px;

    .step {
      gap: 12px;
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      text-align: center;
      margin-bottom: 30px;

      .step-detail {
        font-size: 13px;
        color: rgba(0, 0, 0, 0.8);
        line-height: 1.5;
        max-width: 300px;
      }
    }
  }
}

@media (max-width: 768px) {
  .product-usage-guide {
    .guide-steps {
      grid-template-columns: 1fr;
    }
  }
}

@media (min-width: 768px) and (max-width: 1024px) {
  .product-usage-guide {
    .guide-steps {
      grid-template-columns: repeat(2, 1fr);
    }
  }
}
</style>
