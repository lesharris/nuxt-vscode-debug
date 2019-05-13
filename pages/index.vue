<template>
  <section class="section">
    <div class="container">
      <h1 class="title">
        Let's Debug!
      </h1>
      <h2 class="subtitle">
        Sample Project showing Nuxt.js Debugging in VS Code
      </h2>
      <div class="level">
        <div class="level-item">
          <a class="button is-primary is-large" @click="handleClick">
            Do Arbitrary Action!
          </a>
        </div>
      </div>
      <h1 class="title">
        {{ message }}
      </h1>
    </div>
  </section>
</template>

<script>
export default {
  name: 'IndexView',
  data() {
    return {
      message: ''
    }
  },
  methods: {
    handleClick() {
      this.message = 'Hello from the client!'
    }
  }
}
</script>
