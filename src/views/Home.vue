<template>
  <div class="home">
    <!--<img alt="Vue logo" src="../assets/logo.png">-->
    <LogIn></LogIn>
  </div>
</template>

<script>
// @ is an alias to /src
import LogIn from '@/components/LogIn.vue'

export default {
  name: 'home',
  components: {
    LogIn
  }
}
</script>

<style lang="scss">
@import "../styles/universal.scss";
</style>
