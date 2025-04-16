<script setup lang="ts">
import { ref } from 'vue'
import { Pagination, Autoplay } from 'swiper/modules'
import { Swiper, SwiperSlide } from 'swiper/vue'
import 'swiper/css'
import 'swiper/css/pagination'

const modules = [Pagination, Autoplay]

const ratingList = ref([
  {
    id: '1',
    name: 'Linh Nguyễn',
    job: 'Beauty Blogger',
    image: 'https://placehold.co/400x400?text=Linh',
    text: 'Dùng em serum này 2 tuần là thấy da sáng rõ luôn. Kết cấu mỏng nhẹ, thấm siêu nhanh, không bết dính. Chốt đơn 10 chai nữa nhé!',
  },
  {
    id: '2',
    name: 'Hải Trần',
    job: 'Makeup Artist',
    image: 'https://placehold.co/400x400?text=Hải',
    text: 'Kem nền này xịn thật, che phủ tốt mà vẫn tự nhiên. Đánh lên da không bị cakey, giữ được tone suốt cả ngày.',
  },
  {
    id: '3',
    name: 'Minh Châu',
    job: 'Skincare Enthusiast',
    image: 'https://placehold.co/400x400?text=Châu',
    text: 'Mình da dầu mà dùng kem dưỡng này thấy ổn áp phết. Không bị lên mụn, dưỡng ẩm vừa đủ. Recommend cho bạn nào da hỗn hợp tới dầu.',
  },
  {
    id: '4',
    name: 'Quang Phạm',
    job: 'TikTok Reviewer',
    image: 'https://placehold.co/400x400?text=Quang',
    text: 'Chấm 9/10 cho bạn sữa rửa mặt này! Mùi thơm nhẹ, rửa xong da vẫn mịn không bị khô căng. Gói gọn trong một từ: Đỉnh!',
  },
  {
    id: '5',
    name: 'Trang Lê',
    job: 'Cosmetic Reviewer',
    image: 'https://placehold.co/400x400?text=Trang',
    text: 'Son này lên màu chuẩn lắm, không bị lệch với màu swatch. Chất son mịn, không làm khô môi, packaging nhìn cũng sang xịn mịn nữa.',
  },
])
</script>

<template>
  <div id="rating" class="component-container product-ratings-container detail-component">
    <h1 class="title">ĐÁNH GIÁ CỦA KHÁCH HÀNG</h1>
    <p class="subtitle">
      Lorem ipsum madolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor coli
      incididunt ut labore Lorem ipsum madolor sit amet.
    </p>
    <section class="section product-ratings">
      <swiper
        :modules="modules"
        :slides-per-view="3"
        :space-between="30"
        :pagination="{ clickable: true }"
        :autoplay="{ delay: 5000, disableOnInteraction: false }"
        :breakpoints="{
          320: { slidesPerView: 1, spaceBetween: 10 }, // Mobile: 1 image
          768: { slidesPerView: 2, spaceBetween: 15 }, // Tablet: 2 images
          1024: { slidesPerView: 3, spaceBetween: 20 }, // Desktop: 3 images
        }"
      >
        <swiper-slide class="rating-item" v-for="ratingItem in ratingList" :key="ratingItem.id">
          <div class="rating-text">
            <q>{{ ratingItem.text }}</q>
          </div>
          <div class="rating-author">
            <img :src="ratingItem.image" alt="" />
            <div class="author-info">
              <p class="name">{{ ratingItem.name }}</p>
              <p class="job">{{ ratingItem.job }}</p>
            </div>
          </div>
        </swiper-slide>
      </swiper>
    </section>
  </div>
</template>

<style scoped>
.swiper-slide {
  display: flex !important;
  justify-content: center !important;
  align-items: center !important;
}

:deep(.swiper-pagination) {
  margin-top: 30px;
  position: relative;
}

.product-ratings {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 7rem;

  .rating-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 2rem;
    max-width: 420px;

    .rating-text {
      background-color: #e6e9ec;
      padding: 20px;
      height: 200px;
      text-align: center;
      display: flex;
      align-items: center;
      justify-content: center;

      q {
        font-family: var(--roboto-font);
        font-style: italic;
        font-weight: 400;
        line-height: 1.8em;
        font-size: 18px;
      }
    }

    .rating-author {
      display: flex;
      gap: 1rem;
      align-items: center;

      img {
        height: 50px;
        width: 50px;
        border-radius: 50%;
      }

      .author-info {
        font-size: 14px;

        .name {
          font-weight: bold;
          margin-bottom: 6px;
        }

        .job {
          color: #ff8300;
          font-family: var(--roboto-condensed-font);
        }
      }
    }
  }
}
</style>
