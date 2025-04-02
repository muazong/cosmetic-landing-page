<script setup lang="ts"></script>

<template>
  <section id="product-ingredients">
    <h1>THÀNH PHẦN</h1>
    <div class="product-ingredients-container">
      <ul class="list">
        <li class="item">
          <img src="@/assets/images/ingredient/vitamin-c.png" alt="" />
          <div class="text">
            <b>VITAMIN C</b>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, beatae.</p>
          </div>
        </li>
        <li class="item">
          <img src="@/assets/images/ingredient/niacindamide.png" alt="" />
          <div class="text">
            <b>NIACINDAMIDE</b>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, beatae.</p>
          </div>
        </li>
        <li class="item">
          <img src="@/assets/images/ingredient/adenosine.png" alt="" />
          <div class="text">
            <b>ADENOSINE</b>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, beatae.</p>
          </div>
        </li>
      </ul>

      <img src="@/assets/images/thanh-phan.png" alt="" />

      <ul class="list">
        <li class="item">
          <img src="@/assets/images/ingredient/zino.png" alt="" />
          <div class="text">
            <b>ZINO OXIDE</b>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, beatae.</p>
          </div>
        </li>
        <li class="item">
          <img src="@/assets/images/ingredient/allantoin.png" alt="" />
          <div class="text">
            <b>ALLANTOIN</b>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, beatae.</p>
          </div>
        </li>
        <li class="item">
          <img src="@/assets/images/ingredient/omega.png" alt="" />
          <div class="text">
            <b>OMEGA 369</b>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Odio, beatae.</p>
          </div>
        </li>
      </ul>
    </div>
  </section>
</template>

<style scoped>
#product-ingredients {
  width: 100%;
  height: 90vh;
  background-color: #fff;
  padding: 0 40px;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 6rem;
}

.product-ingredients-container {
  max-width: 1100px;
  display: flex;
  align-items: center;
}

.list {
  .item {
    display: flex;
    align-items: center;
    margin-bottom: 36px;
    gap: 12px;

    img {
      height: 60px;
      width: 60px;
    }

    .text {
      display: flex;
      flex-direction: column;
      gap: 8px;

      p {
        font-size: 13px;
      }
    }
  }
}
</style>
