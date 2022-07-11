<template>
  <section class="container">
      <p>{{ message }}</p>

      <router-link to="/price">Price Page</router-link>
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
