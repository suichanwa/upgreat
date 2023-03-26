<template>
  <div>
    <Header />
    <div class="row">
      <div class="col-md-3">
        <Sidebar />
      </div>
      <div class="col-md-6">
        <h1>Welcome to the Kolesa Group Developer Roadmap</h1>
        <p>Select a level of expertise to view the requirements:</p>
        <ul>
          <li>
            <nuxt-link to="/intern">Intern</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/junior">Junior</nuxt-link>
          </li>
          <li>
            <nuxt-link to="/middle">Middle</nuxt-link>
          </li>
        </ul>
      </div>
      <right-side>
        <Dashboard :data="dashboardData" />
      </right-side>
    </div>
  </div>
</template>

<script>
import UserProfile from '~/components/UserProfile.vue'
import Header from '~/components/Header.vue'
import Sidebar from '~/components/Sidebar.vue'
import Dashboard from './Dashboard.vue'
import ProfileSection from '~/components/ProfileSection.vue'
import RightSide from '~/components/RightSide.vue'

export default {
  name: 'Index',
  components: {
    UserProfile,
    Header,
    Sidebar,
    Dashboard,
    ProfileSection,
    RightSide
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
