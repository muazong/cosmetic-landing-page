<script setup lang="ts"></script>

<template>
  <section id="product-feature">
    <h1>BỘT LÀM SÁNG DA VITABRID C12</h1>
    <div class="product-feature-container">
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
        <img src="@/assets/images/intro.png" alt="intro" />
      </div>
    </div>
  </section>
</template>

<style scoped>
#product-feature {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  padding: 0 40px;
  gap: 3rem;
  background-color: #ffffff;
}

.product-feature-container {
  max-width: 1240px;

  .information {
    display: flex;
    align-items: center;
    justify-content: space-evenly;

    .text {
      max-width: 560px;
      p {
        line-height: 1.4;
        font-size: 14px;
        margin: 16px 0;
        text-align: justify;
      }
    }
  }
}
</style>
