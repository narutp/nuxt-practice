<template>
  <div class = "container">
    <h1>Information...</h1>
    <h3>testing 2 button with different code that route to home page</h3>
    <div>
      <button type="primary" @click="homeClicked()">Home1</button>
      <button type="primary" @click="homeClicked2()">Home2</button>
      <button type="primary" @click="isModal = true">Show Modal</button>
    </div>
    <div class="modal" v-if="isModal" width="500px">
      <div class="modal-background"></div>
      <div class="modal-content">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna
      </div>
      <button class="modal-close is-large"></button>
    </div>
  </div>
</template>
<script>
export default {
  data () {
    return {
      isModal: false
    }
  },
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
