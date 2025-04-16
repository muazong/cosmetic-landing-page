<script setup lang="ts">
import { ref, watch } from 'vue'
const isModelOpen = ref<boolean>(false)

watch(isModelOpen, (newValue) => {
  if (newValue) {
    document.body.classList.add('no-scroll')
  } else {
    document.body.classList.remove('no-scroll')
  }
})

function scrollToSection(event: Event, id: string) {
  event.preventDefault()

  isModelOpen.value = false
  const element = document.getElementById(id)
  if (element) {
    element.scrollIntoView()
  }
}
</script>

<template>
  <div class="component-container nav-container">
    <nav class="nav section">
      <h1 class="nav-logo">
        <a href="#home" @click="scrollToSection($event, 'home')">VITABRID</a>
      </h1>

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

      <button class="nav-contact-btn"><a href="#contact">Liên hệ</a></button>

      <button class="nav-menu-icon" @click="isModelOpen = true">
        <i class="pi pi-bars"></i>
      </button>
    </nav>

    <div :class="['nav-modal', { isOpen: isModelOpen }]">
      <button class="close-btn" @click="isModelOpen = false">&times;</button>
      <ul class="nav-modal-btns">
        <li class="nav-modal-btn">
          <a href="#home" @click="scrollToSection($event, 'home')">Trang chủ</a>
        </li>
        <li class="nav-modal-btn">
          <a href="#detail" @click="scrollToSection($event, 'detail')">Chi tiết</a>
        </li>
        <li class="nav-modal-btn">
          <a href="#award" @click="scrollToSection($event, 'award')">Giải thưởng</a>
        </li>
        <li class="nav-modal-btn">
          <a href="#rating" @click="scrollToSection($event, 'rating')">Đánh giá</a>
        </li>
        <li class="nav-modal-btn">
          <a href="#contact" @click="scrollToSection($event, 'rating')">Liên hệ</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style scoped>
.nav-container {
  top: 0;
  right: 0;
  left: 0;
  position: fixed;
  z-index: 99;
  background: rgba(255, 255, 255, 0.29);
  box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
  backdrop-filter: blur(7.8px);
  -webkit-backdrop-filter: blur(7.8px);
}

.nav {
  height: var(--nav-height);
  display: flex;
  align-items: center;
  justify-content: space-between;

  .nav-logo {
    a {
      color: #3e3f5b;
    }
  }

  .nav-btns {
    display: flex;
    align-items: center;
    gap: 2rem;

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
  }

  .nav-contact-btn {
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

  .nav-menu-icon {
    display: flex;
    align-items: center;
    justify-content: center;
    background: none;
    font-size: 1.3rem;
    display: none;
    cursor: pointer;
  }
}

.nav-modal {
  position: absolute;
  top: 0;
  width: 100%;
  height: 100vh;
  z-index: 99;
  display: none;
  background: rgba(0, 0, 0, 0.48);
  box-shadow: 0 4px 30px rgba(0, 0, 0, 0.1);
  backdrop-filter: blur(4.9px);
  -webkit-backdrop-filter: blur(4.9px);

  .close-btn {
    position: absolute;
    right: 20px;
    background: none;
    color: #fff;
    font-size: 3rem;
    cursor: pointer;
  }

  .nav-modal-btns {
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    gap: 12px;

    .nav-modal-btn {
      font-size: 1.4rem;
    }
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

@media (max-width: 768px) {
  .nav {
    padding: 0 20px;
    .nav-btns {
      display: none;
    }

    .nav-contact-btn {
      display: none;
    }

    .nav-menu-icon {
      display: block;
    }
  }

  .nav-modal.isOpen {
    display: block;
  }
}
</style>
