<script setup>
import { ref } from "vue";
import { Icon } from "@iconify/vue";

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
      <!-- Logo -->
      <div class="Header-Logo">
        <img :src="Logo" alt="HH-Soft" />
      </div>

      <!-- Navigation -->
      <nav class="Navbar">
        <a href="#">BIM-контент</a>
        <a href="#">Сопровождение BIM проектов</a>
        <a href="#">Обучение</a>
        <a href="#">Контакты</a>
      </nav>

      <!-- Right Side -->
      <div class="Header-Right">
        <!-- Social Media -->
        <div class="Header-Social-Media">
          <a href="#" class="social vk">
            <Icon icon="ri:vk-fill" />
          </a>

          <a href="#" class="social youtube">
            <Icon icon="ri:youtube-fill" />
          </a>

          <a href="#" class="social telegram">
            <Icon icon="ri:telegram-fill" />
          </a>
        </div>

        <!-- Phone -->
        <a href="tel:+79826232617" class="Phone"> +7 (982) 623 26 17 </a>

        <!-- Burger -->
        <button class="Burger" @click="toggleMenu">
          <span></span>
          <span></span>
          <span></span>
        </button>
      </div>
    </div>

    <!-- Mobile Menu -->
    <div class="MobileMenu" :class="{ active: isOpen }">
      <a href="#">BIM-контент</a>
      <a href="#">Сопровождение BIM проектов</a>
      <a href="#">Обучение</a>
      <a href="#">Контакты</a>
    </div>
  </header>
</template>
