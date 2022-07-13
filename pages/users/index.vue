<template>
  <section class="container">
    <h1>/users/index.vue</h1>
    <input type="number" v-model="idNum" id="id-num">
    <router-link :to="{name: 'users-id', params: {id: idNum}}">User Page</router-link>
    <br><br>
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

<style>
  #id-num {
    width: 50px;
  }
</style>
