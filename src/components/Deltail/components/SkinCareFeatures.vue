<script setup lang="ts"></script>

<template>
  <section id="skin-care-features">
    <div class="skin-care-features-container">
      <div class="skin-care-features-item">
        <img src="@/assets/images/skin-care-1.jpg" alt="Skin care 1" />
        <h3>GIẢM MỤN, MỜ THÂM</h3>
      </div>
      <div class="skin-care-features-item">
        <img src="@/assets/images/skin-care-2.jpg" alt="Skin care 2" />
        <h3>ĐẨY LÙI LÃO HÓA</h3>
      </div>
      <div class="skin-care-features-item">
        <img src="@/assets/images/skin-care-3.jpg" alt="Skin care 3" />
        <h3>DƯỠNG DA TRẮNG SÁNG</h3>
      </div>
    </div>
  </section>
</template>

<style scoped>
#skin-care-features {
  align-items: center;
  display: flex;
  height: 60vh;
  justify-content: center;
  padding: 0 40px;
  width: 100%;

  .skin-care-features-container {
    align-items: center;
    background-color: #fff;
    display: flex;
    gap: 20px;
    justify-content: space-between;
    max-width: 1240px;

    .skin-care-features-item {
      display: flex;
      align-items: center;
      justify-content: center;
      flex-direction: column;
      gap: 16px;

      img {
        width: 100%;
        height: 260px;
        object-fit: cover;
        border-radius: 12px;
        box-shadow: 0 0 5px 2px rgba(0, 0, 0, 0.2);
      }

      h3 {
        text-align: center;
      }
    }
  }
}
</style>
