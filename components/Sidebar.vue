<template>
  <nav class="navbar bg-light">
    <div class="input-group">
      <div class="input-group-prepend">
        <span class="input-group-text" id="basic-addon1">
          <i class="fa fa-search"></i>
        </span>
      </div>
      <input type="text" class="form-control" placeholder="Search" aria-label="Search" aria-describedby="basic-addon1">
    </div>
    <ul class="nav flex-column mt-3">
      <li class="nav-item">
        <nuxt-link class="nav-link active" to="/intern">
          <i class="fas fa-code-branch"></i>
          <span>Intern</span>
        </nuxt-link>
      </li>
      <li class="nav-item">
        <nuxt-link class="nav-link" to="/junior">
          <i class="fas fa-user-graduate"></i>
          <span>Junior</span>
        </nuxt-link>
      </li>
      <li class="nav-item">
        <nuxt-link class="nav-link" to="/middle">
          <i class="fas fa-user-tie"></i>
          <span>Middle</span>
        </nuxt-link>
      </li>
      <li class="nav-item">
        <nuxt-link class="nav-link" to="/senior">
          <i class="fas fa-user-tie"></i>
          <span>Senior</span>
        </nuxt-link>
      </li>
    </ul>
  </nav>
</template>


<script>
import Dashboard from '../pages/Dashboard.vue';

export default {
  name: 'Sidebar',
  components: {
    Dashboard
  },
  data() {
    return {
      user: {
        name: 'John Doe',
        profilePicture: 'https://placekitten.com/200/200',
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
  width: 4rem;
  height: 4rem;
  border-radius: 50%;
}
</style>
