<script setup>
import "./Main2.css";

const services = [
  {
    title: "Сопровождение BIM проектов",
    text: "Осуществляем анализ технического задания на BIM-проектирование и сопровождение проектов."
  },
  {
    title: "Внедрение BIM",
    text: "Помогаем внедрить BIM в компанию используя многолетний опыт наших специалистов."
  },
  {
    title: "Обучение проектировщиков",
    text: "Обучаем работе с BIM технологиями, Autodesk Revit и Dynamo."
  },
  {
    title: "Создание BIM библиотек",
    text: "Разрабатываем BIM-модели, семейства, шаблоны и стандарты компании."
  },
  {
    title: "Разработка плагинов",
    text: "Создаем плагины, скрипты и программные решения для автоматизации."
  },
  {
    title: "Перевод документации",
    text: "Преобразование 2D чертежей в полноценные BIM модели."
  }
];
</script>

<template>
  <section id="main2">
    <div class="main2">
      <div class="section-title">
        <h1>НАШИ УСЛУГИ</h1>
      </div>

      <div class="main2-cards">
        <div
          class="main2-card"
          v-for="(item, index) in services"
          :key="index"
        >
          <div class="card-icon">
            BIM
          </div>

          <h2>{{ item.title }}</h2>

          <p>
            {{ item.text }}
          </p>

          <a href="#">Подробнее</a>

          <button>
            Оставить заявку
          </button>
        </div>
      </div>
    </div>
  </section>
</template>