<template>
  <div class="navigation">
    <button class="btn btn-primary" @click="goBack">Back</button>
    <button class="btn btn-primary" @click="goNext">Next</button>
  </div>
</template>

<script>
export default {
  name: 'Navigation',
  props: {
    currentPage: {
      type: String,
      required: true
    }
  },
  methods: {
    goBack() {
      const previousPage = this.getPreviousPage();
      if (previousPage) {
        this.$router.push(previousPage);
      }  
      else {
        this.$router.push('/');
      }
    },
    goNext() {
      const nextPage = this.getNextPage();
      if (nextPage) {
        this.$router.push(nextPage);
      }  
      else {
        this.$router.push('/');
      }
    },
    getPreviousPage() {
      switch (this.currentPage) {
        case 'Intern':
          return null; // no previous page for Intern
        case 'Junior':
          return '/intern';
        case 'Middle':
          return '/junior';
        default:
          return null;
      }
    },
    getNextPage() {
      switch (this.currentPage) {
        case 'Intern':
          return '/junior';
        case 'Junior':
          return '/middle';
        case 'Middle':
          return null; // no next page for Middle
        default:
          return null;
      }
    }
  }
};
</script>

<style scoped>
.navigation {
  display: flex;
  justify-content: space-between;
  margin-top: 1rem;
}
</style>
