<template>
  <section class="container">
    <h1>{{ message }}</h1>
    <p>id: {{ this.$route.params.id }}</p>
    <button @click="back()">Back</button>
  </section>
</template>

<script>
  export default {
    data: () => ({
      message: '/users/_id.vueを表示中'
    }),
    validate({ params }) {
      // 数値判定
      return /^\d+$/.test(params.id)
    },
    methods: {
      // ブラウザバック
      back () {
        this.$router.back()
      }
    }
  }
</script>
