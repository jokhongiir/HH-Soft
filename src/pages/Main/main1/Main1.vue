<script setup>
import laptop from "../../../assets/laptop.png";
import Video from "../../../assets/Услуги HH SOFT.mp4";
import "./Main1.css";
</script>

<template>
  <section id="Main1">
    <div class="Main1-Container">
      <!-- Left Content -->
      <div class="Main1-Content">
        <h1>
          РАСТИМ ПОКАЗАТЕЛИ
          <br />
          ВАШЕГО БИЗНЕСА
        </h1>

        <p>
          У всех наших BIM менеджеров опыт работы с компаниями более 10 лет.
          Поэтому мы превращаем наш многолетний опыт BIM в ваш успех.
        </p>

        <div class="Main1-Buttons">
          <button class="PrimaryBtn">Обсудить проект</button>

          <button class="SecondaryBtn">Выбрать курс</button>
        </div>
      </div>

      <!-- Right Side Laptop -->
      <div class="Main1-Image">
        <div class="Glow Glow1"></div>
        <div class="Glow Glow2"></div>
        <div class="Glow Glow3"></div>

        <div class="LaptopWrapper">
          <!-- YOUTUBE VIDEO -->
          <iframe
            class="LaptopVideo"
            src="https://www.youtube.com/embed/dJXEuYKqFv4?autoplay=1&mute=1&loop=1&playlist=dJXEuYKqFv4&controls=0&rel=0"
            title="HH SOFT Video"
            frameborder="0"
            allow="
              accelerometer;
              autoplay;
              clipboard-write;
              encrypted-media;
              gyroscope;
              picture-in-picture;
            "
            allowfullscreen
          >
          </iframe>

          <!-- LAPTOP FRAME -->
          <img :src="laptop" alt="HH SOFT Laptop" class="LaptopFrame" />
        </div>
      </div>
    </div>
  </section>
</template>
