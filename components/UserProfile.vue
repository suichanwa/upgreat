<template>
  <div class="user-profile">
    <img :src="user.profilePicture" alt="User Profile Picture" class="profile-picture">
    <div class="user-info">
      <h2 class="username">{{ user.name }}</h2>
      <p class="user-level">Level {{ user.level }}</p>
    </div>
  </div>
</template>

<script>
export default {
  name: 'UserProfile',
  props: {
    user: {
      type: Object,
      required: true
    }
  }
}
</script>

<style scoped>
.user-profile {
  display: flex;
  align-items: center;
  margin: 1rem;
}

.profile-picture {
  width: 4rem;
  height: 4rem;
  border-radius: 50%;
  margin-right: 1rem;
}

.username {
  margin: 0;
}

.user-level {
  margin: 0;
  font-weight: bold;
}
</style>
