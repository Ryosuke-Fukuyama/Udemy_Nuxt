<template>
  <section class="container">
    <h1>/users/index.vue</h1>
    <input type="number" v-model="idNum">
    <router-link :to="{name: 'users-id', params: {id: idNum}}">User Page</router-link>
    <router-link to="/">Top Page</router-link>
  </section>
</template>

<script>
  export default {
    data: () => ({
      idNum: 0
    }),
  }
</script>
