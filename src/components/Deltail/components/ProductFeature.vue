<script setup lang="ts"></script>

<template>
  <div class="component-container product-feature-container detail-component">
    <h1 class="title">BỘT LÀM SÁNG DA VITABRID C12</h1>
    <section class="section product-feature">
      <div class="information">
        <div class="text">
          <p>
            Vitamin C gần như có thể giải quyết được mọi vấn đề về da như sạm da, thâm nám, lão hoá,
            đồng thời bảo vệ da theo cơ chế tự nhiên, giúp da đẹp trên nền tảng da khoẻ. Vitamin C
            thẩm thấu và hoạt động tốt nhất trên da khi ở dạng nguyên chất Ascorbic Acid. Tuy nhiên,
            Vitamin C nguyên chất dạng Ascorbic Acid thông thường khó hấp thụ vào da do dễ oxy hoá
            và bay hơi, dễ gây kích ứng cho da nhạy cảm, không thể dùng ở liều lượng cao.
          </p>
          <p>
            Bột vitamin C Bột làm sáng da Vitabrid C12 - với công nghệ LDH độc quyền của tập đoàn
            Hyundai Bioscience - không những khắc phục mà còn tối ưu triệt để loại vitamin giàu năng
            lượng này: tăng sinh collagen, giảm hắc tố melanin, ngăn chặn gốc tự do, phòng ngừa tác
            hại tia UV. Bạn không cần phải lích kích chai lọ bảo quản, lo lắng vitamin C bị oxy hóa
            quá nhanh trước khi dùng hết hay phải bôi thêm 1 lớp dưỡng trong chu trình skincare. Chỉ
            cần trộn bột cùng toner/serum rồi thoa lên da, bạn đã cung cấp đủ lượng vitamin C cho da
            trong suốt 12h liên tục.
          </p>
        </div>
        <img class="product-image" src="@/assets/images/intro.png" alt="intro" />
      </div>
    </section>
  </div>
</template>

<style scoped>
.product-feature-container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  gap: 3rem;
  background-color: #ffffff;
}

.product-feature {
  .information {
    display: flex;
    align-items: center;
    justify-content: space-between;

    .text {
      p {
        line-height: 1.5;
        font-size: 14px;
        font-weight: 300;
        margin: 16px 0;
        text-align: justify;
      }
    }

    .product-image {
      margin-top: -80px;
    }
  }
}

@media (max-width: 768px) {
  .product-feature {
    .information {
      flex-direction: column;

      .product-image {
        margin-top: unset;
        height: 300px;
      }
    }
  }
}

@media (min-width: 768px) and (max-width: 1024px) {
  .product-feature {
    .information {
      .product-image {
        height: 400px;
      }
    }
  }
}
</style>
