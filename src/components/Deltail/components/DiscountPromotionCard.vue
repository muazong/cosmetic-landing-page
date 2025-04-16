<script setup lang="ts">
import BuyButton from './BuyButton.vue'
</script>

<template>
  <div class="discount-promotion-card-container">
    <section class="section discount-promotion-card">
      <div class="discount-promotion-card-content">
        <h2 class="title">ƯU ĐÃI DÀNH RIÊNG CHO BẠN</h2>
        <div class="prices">
          <p class="old-price">1.490.000đ</p>
          <p class="new-price">1.290.000đ</p>
        </div>
        <div class="text">
          <p>
            Khi mua 1 hộp Vitabrid C12 giá <mark>1.490.000đ</mark> nay giảm còn
            <mark>1.390.000đ</mark>. <br />
            <strong>Lưu ý:</strong> thời gian ưu đãi chỉ còn:
          </p>
        </div>
        <BuyButton text="ĐẶT MUA NGAY" />
      </div>
      <img class="product" src="@/assets/images/banner-1.png" alt="" />
    </section>
  </div>
</template>

<style scoped>
.discount-promotion-card-container {
  height: 100vh;
  overflow: hidden;
  background: linear-gradient(45deg, #1dcdf4, #84ec9f);
  display: flex;
  align-items: center;
  justify-content: center;
}

.discount-promotion-card {
  display: flex;
  align-items: center;
  justify-content: center;

  .discount-promotion-card-content {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 1.4rem;

    .title {
      color: #ffffff;
    }

    .prices {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 2rem;

      p {
        padding: 4px 26px;
        font-weight: bold;
        font-size: 32px;
        color: #ffffff;
        background-color: #014973;
      }

      .old-price {
        text-decoration: line-through;
      }
    }

    .text {
      font-size: 13px;
      text-align: center;

      mark {
        color: #ffffff;
        font-weight: bold;
        background-color: #ffcc00;
      }
    }
  }

  .product {
    width: 60%;
    margin-bottom: -220px;
  }
}
</style>
