<template>
  <div class="container mt-5">
    <div class="card">
      <div class="card-body">
        <h2 class="card-title">Требования для Junior Разработчика</h2>
        <h4>Junior - это следующий шаг на дорожной карте разработчика. Разработчик становится полноценным членом нашей команды, который отныне имеет чёткие полномочия и обязанности.</h4>
        <ul>
          <h5>Hard Skills</h5>
          <li><ul><h6>Опыт использования языка программирования PHP</h6> 
            <li>Базовое знание синтаксиса, типов данных и понимание концепций объектно-ориентированного программирования</li>
          <li>Базовые навыки в HTML и CSS</li>
          </ul></li>
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

