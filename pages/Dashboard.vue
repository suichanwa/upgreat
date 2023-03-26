<template>
  <div class="container">
    <Header/>
    <h1>Dashboard</h1>
    <div class="card mb-3">
      <div class="card-header">My Progress</div>
      <div class="card-body">
        <p>Here's your progress:</p>
        <ul>
          <li>Completed lessons: {{ completedLessons }}</li>
          <li>Lessons in progress: {{ lessonsInProgress }}</li>
          <li>Total lessons: {{ totalLessons }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
import Header from '~/components/Header.vue'
export default {
  name: 'Dashboard',
  computed: {
    completedLessons() {
      // Calculate the number of completed lessons based on data from your backend
      // This is just an example, you would need to implement this yourself
      return 10;
    },
    lessonsInProgress() {
      // Calculate the number of lessons in progress based on data from your backend
      // This is just an example, you would need to implement this yourself
      return 5;
    },
    totalLessons() {
      // Calculate the total number of lessons based on data from your backend
      // This is just an example, you would need to implement this yourself
      return 20;
    }
  }
};
</script>
<style scoped>
h1{
  margin: 20px 0;
  padding: auto;
  box-sizing: border-box;
}
</style>