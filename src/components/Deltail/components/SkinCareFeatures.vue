<script setup lang="ts"></script>

<template>
  <div class="component-container skin-care-features-container detail-component">
    <section class="section skin-care-features">
      <div class="skin-care-features-image">
        <img src="@/assets/images/skin-care-1.jpg" alt="Skin care 1" />
        <h3>GIẢM MỤN, MỜ THÂM</h3>
      </div>
      <div class="skin-care-features-image">
        <img src="@/assets/images/skin-care-2.jpg" alt="Skin care 2" />
        <h3>ĐẨY LÙI LÃO HÓA</h3>
      </div>
      <div class="skin-care-features-image">
        <img src="@/assets/images/skin-care-3.jpg" alt="Skin care 3" />
        <h3>DƯỠNG DA TRẮNG SÁNG</h3>
      </div>
    </section>
  </div>
</template>

<style scoped>
.skin-care-features {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  max-width: 1200px;
  gap: 16px;
  padding-top: var(--nav-height);
}

.skin-care-features-image {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  text-align: center;

  img {
    width: 100%;
    max-width: 370px;
    height: 280px;
    object-fit: cover;
    border-radius: 12px;
    box-shadow: 0 0 5px 2px rgba(0, 0, 0, 0.2);
    margin-bottom: 22px;
  }

  h3 {
    font-size: 1.2rem;
  }
}
</style>
