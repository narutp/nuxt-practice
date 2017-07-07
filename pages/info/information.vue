<template>
  <div class = "container">
    <h1>Information... testing 2 button with different code that route to home page</h1>
    <button type="primary" @click="homeClicked()">Home1</button>
    <button type="primary" @click="homeClicked2()">Home2</button>
  </div>
</template>
<script>
export default {
  methods: {
    homeClicked () {
      this.$router.replace({ path: '/' })
    },
    homeClicked2 () {
      window.location.href = '/'
    }
  }
}
</script>
