<script setup>
import { ref } from "vue";
import "./Header.css";
import Logo from "../../assets/HH-Soft-Logo.png";

const isOpen = ref(false);

const toggleMenu = () => {
  isOpen.value = !isOpen.value;
};
</script>

<template>
  <header class="Header">
    <div class="Header-Container">
      <div class="Header-Logo">
        <img :src="Logo" alt="HH-Soft" />
      </div>

      <nav class="Navbar">
        <a href="#">BIM-контент</a>
        <a href="#" class="active">Сопровождение BIM проектов</a>
        <a href="#">Обучение</a>
        <a href="#">Контакты</a>
      </nav>

      <div class="Header-Right">
        <div class="Header-Social-Media">
          <a href="#" class="social vk">
            <i class="fab fa-vk"></i>
          </a>

          <a href="#" class="social youtube">
            <i class="fab fa-youtube"></i>
          </a>

          <a href="#" class="social telegram">
            <i class="fab fa-telegram-plane"></i>
          </a>
        </div>

        <a href="tel:+79826232617" class="Phone">
          +7 (982) 623 26 17
        </a>

        <button class="Burger" @click="toggleMenu">
          <span></span>
          <span></span>
          <span></span>
        </button>
      </div>
    </div>

    <div class="MobileMenu" :class="{ active: isOpen }">
      <a href="#">BIM-контент</a>
      <a href="#">Сопровождение BIM проектов</a>
      <a href="#">Обучение</a>
      <a href="#">Контакты</a>
    </div>
  </header>
</template>