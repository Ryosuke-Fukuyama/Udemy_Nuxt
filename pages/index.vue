<template>
  <section class="container">
      <p>{{ message }}</p>

      <router-link to="/users/">Users Index</router-link>
      <router-link to="/users/other">Users Other</router-link>
  </section>
</template>

<script>
export default {
  // name: 'IndexPage'
  data: () => ({
    message: 'Hello Nuxt.js!'
  })
}
</script>

<style>
  p {
    font-family: 'Edu VIC WA NT Beginner', cursive;
  }
</style>
