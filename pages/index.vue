<template>
  <div>
    <Header />
    <div class="container">

      <div>
        <logo />
        <h1 class="title change_font">
          Black Dragon
        </h1>
        <h2 class="subtitle change_font">
          My history &amp; Technology
        </h2>
        <div class="links">
          <a
            href="https://twitter.com/bzg_white"
            target="_blank"
            class="button--white"
          >
          Twitter
          </a>
          <a
            href="https://github.com/bzgwhite"
            target="_blank"
            class="button--white"
          >
            GitHub
          </a>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>

<script lang="ts">
import Logo from '@/components/Logo.vue'

export default ({
  components: {
    Logo
  }
})
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
  color: #d3d5d8;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #e7eaf0;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
