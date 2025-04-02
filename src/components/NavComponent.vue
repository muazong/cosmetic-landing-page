<script setup lang="ts">
const scrollToSection = (event: Event, id: string) => {
  event.preventDefault()

  const element = document.getElementById(id)
  if (element) {
    element.scrollIntoView()
  }
}
</script>

<template>
  <nav id="navigation">
    <div class="navigation-container">
      <h1 class="logo"><a href="#home">VITABRID</a></h1>
      <ul class="nav-btns">
        <li class="nav-btn">
          <a href="#home" @click="scrollToSection($event, 'home')">Trang chủ</a>
        </li>
        <li class="nav-btn">
          <a href="#detail" @click="scrollToSection($event, 'detail')">Chi tiết</a>
        </li>
        <li class="nav-btn">
          <a href="#award" @click="scrollToSection($event, 'award')">Giải thưởng</a>
        </li>
        <li class="nav-btn">
          <a href="#rating" @click="scrollToSection($event, 'rating')">Đánh giá</a>
        </li>
      </ul>
      <button class="contact-btn"><a href="#contact">Liên hệ</a></button>
    </div>
  </nav>
</template>

<style scoped>
#navigation {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  position: fixed;
  top: 0;
  z-index: 99;
  padding: 0 40px;
  background: rgba(255, 255, 255, 0.29);
  box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
  backdrop-filter: blur(7.8px);
  -webkit-backdrop-filter: blur(7.8px);
}

.navigation-container {
  width: 100%;
  height: 56px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  max-width: 1240px;
  border-bottom: 1px solid rgba(0, 0, 0, 0.2);
}

.logo {
  a {
    color: #3e3f5b;
  }
}

.nav-btns {
  display: flex;
  align-items: center;
  gap: 2rem;
}

.nav-btn {
  font-size: 16px;
  font-weight: bold;
  position: relative;

  &:hover {
    a::after {
      display: block;
    }
  }

  a {
    color: #1f1f1f;

    &::after {
      content: '';
      position: absolute;
      width: 100%;
      height: 2px;
      background-color: #3e3f5b;
      bottom: 0;
      transform: scaleX(0);
      transform-origin: center;
      display: none;
      animation: spread 0.3s ease forwards;
    }
  }
}

.contact-btn {
  font-size: 15px;
  font-weight: bold;
  padding: 6px 12px;
  border-radius: 4px;
  background-color: rgba(154, 203, 208, 0.8);
  border: 2px solid #123458;
  transition: all 0.2s ease-in-out;

  a {
    color: #1f1f1f;
  }

  &:hover {
    border: 2px solid #123458;
    background-color: transparent;
    cursor: pointer;
    transform: scale(1.03);
  }
}

@keyframes spread {
  from {
    transform: scaleX(0);
  }
  to {
    transform: scaleX(1);
  }
}
</style>
