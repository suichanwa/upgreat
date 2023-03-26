<template>
  <div class="container mt-5">
    <div class="card">
      <div class="card-body">
        <h5 class="card-title">Requirements for Internship Developer</h5>
        <ul>
        <li>Опыт работы с языком программирования PHP</li>
          <li>Базовый синтаксис языка PHP, знание типов данных и конструкций языка</li>
          <li>Базовые навыки вёрстки (CSS, HTML)</li>
          <li>Опыт работы с Git (pull, commit, push, branch, checkout)</li>
          <li>Понимание объектно-ориентированного программирования (ООП), объекты, классы, интерфейсы</li>
          <li>Понимание архитектурного паттерна Model-View-Controller (MVC)</li>
          <li>Базовый синтаксис языка SQL (select, update, insert, delete)</li>
          <li>Базовое понимание работы операционной системы Linux, включая директории, пользователей</li>
          <li>Умение работать в окружении разработки по SSH</li>
          <li>Умение работать с инструментами разработки, включая IDE (например, PhpStorm или VSCode) и клиенты MySQL (например, DataGrip, HeidiSQL или MySQL Workbench)</li>
        </ul>
        <Navigation :currentPage="'Intern'" />
      </div>
    </div>
  </div>
</template>
<script>
import Navigation from '~/components/Navigation.vue';
import SideBar from '~/components/SideBar.vue';

export default {
  name: 'Intern',
  components: {
    Navigation,
    SideBar
  }
}
</script>