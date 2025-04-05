<script setup lang="ts"></script>

<template>
  <div id="award" class="component-container awards-container detail-component">
    <h1 class="title">GIẢI THƯỞNG & CHỨNG CHỈ</h1>
    <p class="subtitle">
      Lorem ipsum madolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor coli
      incididunt ut labore Lorem ipsum madolor sit amet.
    </p>

    <section class="section product-awards">
      <div class="information">
        <img class="certificate" src="@/assets/images/chung-nhan.png" alt="" />

        <div class="text">
          <p class="title">
            Bột làm sáng da Vitabrid C12 VITABRID C12 tự hào sở hữu nhiều giải thưởng và chứng chỉ
            quốc tế về chất lượng và công nghệ.
          </p>

          <div>
            <p class="awards-text">
              <i class="pi pi-check"></i>
              <span>Donec facilisis velit eu est phasellus consequat quis nostrud</span>
            </p>
            <p class="awards-text">
              <i class="pi pi-check"></i>
              <span>Donec facilisis velit eu est phasellus consequat quis nostrud</span>
            </p>
            <p class="awards-text">
              <i class="pi pi-check"></i>
              <span>Donec facilisis velit eu est phasellus consequat quis nostrud</span>
            </p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
.product-awards {
  .information {
    display: flex;
    align-items: center;
    justify-content: center;

    .text {
      margin-top: 30px;
      .title {
        max-width: 500px;
        font-size: 15px;
        line-height: 1.5;
        margin-bottom: 30px;
      }

      .awards-text {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 12px;
        margin-bottom: 12px;
        font-weight: 300;

        span {
          font-size: 14px;
        }
      }
    }
  }
}

@media (max-width: 768px) {
  .information {
    flex-direction: column;

    .certificate {
      height: 100px;
    }
  }
}

@media (min-width: 768px) and (max-width: 1024px) {
  .information {
    .certificate {
      height: 200px;
    }
  }
}
</style>
