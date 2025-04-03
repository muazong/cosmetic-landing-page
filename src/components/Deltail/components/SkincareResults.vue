<script lang="ts" setup>
import { Pagination, Autoplay, Navigation } from 'swiper/modules'
import { Swiper, SwiperSlide } from 'swiper/vue'
import 'swiper/css'
import 'swiper/css/navigation'
import 'swiper/css/pagination'

const modules = [Pagination, Autoplay, Navigation]

const images = [
  '/src/assets/images/slider/1.jpg',
  '/src/assets/images/slider/2.jpg',
  '/src/assets/images/slider/3.jpg',
  '/src/assets/images/slider/4.jpg',
  '/src/assets/images/slider/1.jpg',
  '/src/assets/images/slider/2.jpg',
]
</script>

<template>
  <div id="component-container skin-care-results-container detail-component">
    <h1 class="title">HÌNH ẢNH SỬ DỤNG THỰC TẾ</h1>
    <section class="section skin-care-results">
      <swiper
        :modules="modules"
        :slides-per-view="3"
        :space-between="30"
        :pagination="{ clickable: true }"
        :navigation="true"
        :autoplay="{ delay: 5000, disableOnInteraction: false }"
        :breakpoints="{
          320: { slidesPerView: 1, spaceBetween: 10 }, // Mobile: 1 image
          768: { slidesPerView: 2, spaceBetween: 15 }, // Tablet: 2 images
          1024: { slidesPerView: 3, spaceBetween: 20 }, // Desktop: 3 images
        }"
        class="image-container"
      >
        <swiper-slide class="image-item" v-for="(image, index) in images" :key="index">
          <img :src="image" :alt="'image-' + index" />
        </swiper-slide>
      </swiper>
    </section>
  </div>
</template>

<style lang="css">
/* Đảm bảo Swiper giữ kích thước hợp lý */
.image-container {
  width: 100%;
  height: auto;
  display: flex;
  justify-content: center;
  align-items: center;
}

/* Định dạng từng slide */
.swiper-slide {
  display: flex !important; /* Căn giữa từng ảnh */
  justify-content: center !important;
  align-items: center !important;
}

/* Định dạng ảnh */
.image-container img {
  width: auto;
  max-width: 100%;
  height: 300px; /* Điều chỉnh chiều cao */
  max-height: 400px;
  object-fit: cover;
  border-radius: 12px;
}

/* Điều chỉnh trên mobile */
@media (max-width: 768px) {
  .image-container img {
    height: 200px;
  }
}
</style>
