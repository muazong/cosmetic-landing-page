<script setup lang="ts"></script>

<template>
  <div class="component-container product-details-container detail-component">
    <h1 class="title">ĐẶC TÍNH</h1>
    <section class="section product-details">
      <img class="product-image" src="@/assets/images/dac-tinh.png" alt="features" />
      <div class="information">
        <p>
          Bột vitamin C Bột làm sáng da Vitabrid C12 - với công nghệ LDH độc quyền của tập đoàn
          Hyundai Bioscience - không những khắc phục mà còn tối ưu triệt để loại vitamin giàu năng
          lượng này: tăng sinh collagen, giảm hắc tố melanin, ngăn chặn gốc tự do, phòng ngừa tác
          hại tia UV.
        </p>

        <ul class="features">
          <li class="feature">
            <i class="icon pi pi-cloud"></i>
            <div class="text">
              <b>KHÔNG BỊ OXY HOÁ</b>
              <p>
                Không bị oxy hoá khi gặp không khí và ánh sáng, khắc phục nhược điểm của vitamin C
                dạng serum thông thường.
              </p>
            </div>
          </li>
          <li class="feature">
            <i class="icon pi pi-ethereum"></i>
            <div class="text">
              <b>KHÔNG GÂY KÍCH ỨNG</b>
              <p>
                Không gây kích ứng kể cả với làn da nhạy cảm nhất hay da mụn nhờ cơ chế trao đổi
                i-on.
              </p>
            </div>
          </li>
          <li class="feature">
            <i class="icon pi pi-sun"></i>
            <div class="text">
              <b>KHÔNG GÂY BẮT NẮNG</b>
              <p>
                Không gây bắt nắng do vitamin C nguyên chất trên da đã được ổn định và bền vững hóa
                trong lớp khoáng kép.
              </p>
            </div>
          </li>
        </ul>
      </div>
    </section>
  </div>
</template>

<style scoped>
.product-details-container {
  background-color: #fff;
  flex-direction: column;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 2rem;
}

.product-details {
  max-width: 1240px;
  display: flex;
  align-items: center;

  .information {
    max-width: 550px;

    p {
      font-size: 14px;
      margin-bottom: 16px;
      text-align: justify;
      line-height: 1.4;
    }

    .features {
      .feature {
        display: flex;
        gap: 12px;
        align-items: center;

        .icon {
          color: #78ec96;
          font-weight: bold;
          font-size: 20px;
          padding: 12px;
          border: 1px solid #78ec96;
          border-radius: 50%;
          background-color: #fff;
          position: relative;
          transition: all 0.3s ease-in-out;

          &:hover {
            border: 1px solid #8f87f1;
            background-color: #8f87f1;
            transform: translateY(8px);
          }
        }

        .text {
          p {
            color: rgba(0, 0, 0, 0.7);
          }
        }
      }
    }
  }
}

@media (max-width: 768px) {
  .product-details {
    flex-direction: column;

    .product-image {
      height: 300px;
    }
  }
}

@media (min-width: 768px) and (max-width: 1024px) {
  .product-details {
    .product-image {
      height: 300px;
    }
  }
}
</style>
