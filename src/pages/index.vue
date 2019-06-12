<template>
  <section class="container">
    <div>
      <logo />
      <h1 class="title">
        nuxt firebase
      </h1>
      <h2 class="subtitle">
        deploy nuxt with ssr to firebase functions
      </h2>
      <div class="links">
        <a
          href="https://firebase.google.com/docs/functions/"
          target="_blank"
          class="button--grey"
        >Firebase functions</a>
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="button--grey"
        >Nuxt.js</a>
        <a
          href="https://github.com/comfuture/nuxt-firebase"
          target="_blank"
          class="button--grey"
        >GitHub</a>
      </div>
    </div>
  </section>
</template>

<script>
import Logo from '~/components/Logo.vue'

export default {
  components: {
    Logo
  }
}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
