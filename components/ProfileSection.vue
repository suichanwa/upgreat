<template>
  <div class="profile-section">
    <h2>Profile Section</h2>
    <div class="list-group">
      <a href="#" class="list-group-item list-group-item-action">
        <Dashboard :data="dashboardData" />
      </a>
    </div>
  </div>
</template>
<script>
import Dashboard from '../pages/Dashboard.vue';

export default {
  name: 'ProfileSection',
  components: {
    Dashboard
  },
  data() {
    return {
      dashboardData: {
        progress: 75,
        completedCourses: 12,
        totalCourses: 16
      }
    }
  }
}
</script>
<style scoped>
.profile-section {
  margin: 1rem;
}
</style>