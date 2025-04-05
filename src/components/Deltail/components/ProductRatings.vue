<script setup lang="ts"></script>

<template>
  <div class="component-container product-ratings-container detail-component">
    <h1 class="title">ĐÁNH GIÁ CỦA KHÁCH HÀNG</h1>
    <p class="subtitle">
      Lorem ipsum madolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor coli
      incididunt ut labore Lorem ipsum madolor sit amet.
    </p>
    <section class="section product-ratings">
      <div class="rating-item">
        <div class="rating-text">
          <q>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus aliquam totam
            eligendi obcaecati! Aperiam maxime, iste sequi porro asperiores eos, laborum quis nisi
            adipisci delectus nemo laudantium non, ipsa recusandae?
          </q>
        </div>
        <div class="rating-author">
          <img src="https://placehold.co/400" alt="" />
          <div class="author-info">
            <p class="name">Ms. Nguyễn Thị C</p>
            <p class="job">Co-Founder Donghoviet.vn</p>
          </div>
        </div>
      </div>
      <div class="rating-item">
        <div class="rating-text">
          <q>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatibus aliquam totam
            eligendi obcaecati! Aperiam maxime, iste sequi porro asperiores eos, laborum quis nisi
            adipisci delectus nemo laudantium non, ipsa recusandae?
          </q>
        </div>
        <div class="rating-author">
          <img src="https://placehold.co/400" alt="" />
          <div class="author-info">
            <p class="name">Ms. Nguyễn Thị C</p>
            <p class="job">Co-Founder Donghoviet.vn</p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<style scoped>
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
      text-align: center;
      background-color: #e6e9ec;
      padding: 20px;

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
