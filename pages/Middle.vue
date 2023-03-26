<template>
  <div class="container mt-5">
    <div class="row">
      <div class="col-md-3">
        <Sidebar />
      </div>
      <div class="col-md-9">
        <div class="card">
          <div class="card-body">
            <h5 class="card-title">Требования для Middle Разработчика</h5>
            <h6 class="card-subtitle mb-2 text-muted">Middle 1</h6>
            <ul>
              <li>Опыт работы с популярными расширениями и библиотеками языка программирования</li>
              <li>Опыт конфигурирования интерпретатора</li>
              <li>Понимание паттернов проектирования, включая внедрение зависимостей и порождающие паттерны</li>
              <li>Полное понимание операционной системы Linux, включая systemd service unit и bash scripting</li>
              <li>Понимание принципов SOLID и DRY</li>
              <li>Базовое понимание Kubernetes, включая deployments, pods и services, а также опыт использования kubectl, docker-compose и cron</li>
              <li>Уверенное использование фреймворка вашего проекта, такого как phalcon, symfony, yii или laravel, и опыт оптимизации запросов к базе данных, применения индексов и использования моков в тестировании</li>
            </ul>
            <h6 class="card-subtitle mb-2 text-muted">Middle 2</h6>
            <ul>
              <li>Опыт написания надежного, расширяемого и тестируемого кода</li>
              <li>Умение выделять часто используемые фрагменты кода в библиотеки</li>
              <li>Опыт расширения функциональности фреймворка и создания и изменения деплой/билд планов для CI/CD</li>
              <li>Опыт создания production-ready Docker образов и изменения Kubernetes манифестов</li>
              <li>Понимание и поддержка микросервисной архитектуры</li>
              <li>Опыт работы с дополнительным языком программирования, таким как Go или Python, а также опыт работы с Elasticsearch для маппинга, индексации и поиска данных</li>
            </ul>
            <h6 class="card-subtitle mb-2 text-muted">Middle 3</h6>
            <ul>
              <li>Понимание паттернов проектирования и Domain-Driven Design</li>
              <li>Опыт оркестрации Docker и работы с Kubernetes</li>
              <li>Умение читать и редактировать Ansible плейбуки и роли</li>
              <li>Понимание принципов разработки RESTful API</li>
              <li>Опыт работы с NoSQL базами данных, такими как MongoDB, Redis, ElasticSearch и RabbitMQ</li>
              <li>Опыт работы с системами мониторинга, такими как Prometheus, Grafana, ELK и Zabbix</li>
              <li>Опыт работы с системами автоматического развертывания, такими как Jenkins, GitLab CI/CD и Ansible</li>
            </ul>
            <Navigation :currentPage="'Middle'" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Sidebar from '@/components/Sidebar'
import Navigation from '@/components/Navigation'

export default {
  name: 'Middle',
  components: {
    Sidebar,
    Navigation
  }
}

</script>