<template>
  <nav class="navbar navbar-expand-lg navbar-light bg-light">
    <a class="navbar-brand" href="/">Upgreat.com</a>
    <button
      class="navbar-toggler"
      type="button"
      data-toggle="collapse"
      data-target="#navbarNav"
      aria-controls="navbarNav"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav mr-auto">
        <!-- Other links... -->
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: 'Header'
};
</script>
<style scoped>
a{
  color:black;
  font-family: Arial, Helvetica, sans-serif;
  font-size: 36px;
  font-weight: 900;
}
</style>