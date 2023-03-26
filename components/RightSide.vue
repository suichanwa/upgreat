<template>
  <div class="col-md-3">
    <div class="list-group">
      <a href="#" class="list-group-item list-group-item-action">
        <img :src="user.profilePicture" alt="User Profile Picture" class="profile-picture">
        <h4>{{ user.name }}</h4>
        <p>Level {{ user.level }}</p>
      </a>
      <a href="#" class="list-group-item list-group-item-action">
        <nuxt-link class="nav-link" to="/dashboard">Dashboard</nuxt-link>
      </a>
    </div>
  </div>
</template>

<script>
import Dashboard from '../pages/Dashboard.vue'

export default {
  name: 'RightSide',
  components: {
    Dashboard
  },
  data() {
    return {
      user: {
        name: 'John Doe',
        profilePicture: 'https://i.imgur.com/wF06y10.png',
        level: 5
      },
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
.profile-picture {
  width: 100%;
  border-radius: 50%;
}
</style>
