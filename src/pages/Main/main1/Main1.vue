<script setup>
import MainBackground from "../../../assets/main-backround.png";
import './Main1.css'
</script>

<template>
  <section id="Main1">
    <div class="Main1-Container">
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

      <div class="Main1-Image">
        <div class="Glow Glow1"></div>
        <div class="Glow Glow2"></div>
        <div class="Glow Glow3"></div>

        <img :src="MainBackground" alt="HH-SOFT" />
      </div>
    </div>
  </section>
</template>
