<template>
  <div id="main-app-container">
    <LoginPage />
  </div>
</template>

<script>
import LoginPage from './components/LoginPage.vue'

export default {
  name: 'App',
  components: {
    LoginPage
  }
}
</script>

<style lang="css" scoped>
#main-app-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

  width: 100vw;
  height: 100vh;

  background-image: url(./assets/Background.png);
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
