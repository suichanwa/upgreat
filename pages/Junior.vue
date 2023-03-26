<template>
  <div class="container mt-5">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">Требования для Junior Разработчика</h5>
        <ul>
          <li>Опыт использования языка программирования PHP</li>
          <li>Базовое знание синтаксиса, типов данных и понимание концепций объектно-ориентированного программирования</li>
          <li>Базовые навыки в HTML и CSS</li>
          <li>Опыт использования Git для контроля версий</li>
          <li>Понимание архитектурного шаблона Model-View-Controller (MVC)</li>
          <li>Базовый синтаксис SQL запросов, включая SELECT, UPDATE, INSERT и DELETE</li>
          <li>Базовое понимание операционной системы Linux, включая структуру каталогов, пользователей и основные команды, такие как cd, ls, cat и ssh</li>
          <li>Умение работать в интегрированных средах разработки (IDE) типа PhpStorm или VSCode, а также с клиентами базы данных MySQL, такими как DataGrip, HeidiSQL или MySQL Workbench</li>
        </ul>
        <Navigation :currentPage="'Junior'" />
      </div>
    </div>
  </div>
</template>
<script>
import Navigation from '../components/Navigation.vue';

export default {
  name: 'Junior',
  components: {
    Navigation
  }
}
</script>

