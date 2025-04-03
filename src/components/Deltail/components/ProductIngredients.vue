<script setup lang="ts"></script>

<template>
  <div class="component-container product-ingredients-container detail-component">
    <h1 class="title">THÀNH PHẦN</h1>
    <section class="section product-ingredients">
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
      <img class="product-image" src="@/assets/images/thanh-phan.png" alt="" />
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
    </section>
  </div>
</template>

<style scoped>
.product-ingredients-container {
  background-color: #fff;
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 3rem;
  margin-bottom: var(--nav-height);
}

.product-ingredients {
  max-width: 1100px;
  display: flex;
  align-items: center;

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
}

@media (max-width: 768px) {
  .product-ingredients {
    flex-direction: column;

    .list {
      .item {
        margin-bottom: 20px;

        img {
          width: 40px;
          height: 40px;
        }

        .text {
          b {
            font-size: 13px;
          }
        }
      }
    }

    .product-image {
      height: 280px;
      order: -1;
    }
  }
}

@media (min-width: 768px) and (max-width: 1024px) {
  .product-ingredients {
    .product-image {
      height: 300px;
    }
  }
}
</style>
