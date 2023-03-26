<template>
  <div class="container mt-5">
    <div class="card">
      <div class="card-body">
        <h2 class="card-title">Requirements for Internship Developer</h2>
        <H4>Интерн - первый шаг на дорожной карте разработчика в Kolesa Group.</H4>
        <ul>
          <H5>Hard Skills</H5>
          <li>Язык программирования (любой)</li>
          <li>Знание что такое PHP и готовность его изучать</li>
          <H5>Обязанности</H5>
          <li>Иметь бешеное желание стать Back-end разработчиком</li>
          <li>Стремительно развиваться</li>
          <li>Быть ответственным</li>
          <li>Уметь формулировать вопросы</li>
          <li>Уметь гуглить</li>
          <li>Взаимодействовать с членами своей команды</li>
          <li>Следовать внутренним правилам разработки программного обеспечения</li>
        </ul>
        <Navigation :currentPage="'Intern'" />
      </div>
    </div>
  </div>
</template>

<script>
import Navigation from '~/components/Navigation.vue';

export default {
  name: 'Intern',
  components: {
    Navigation
  }
}
</script>
