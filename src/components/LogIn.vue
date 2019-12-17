<template>
  <div class="LogIn">
    <transition name="fade">
<section class="log-in" v-if="isShow['Log']">
  <h2>please sign in</h2>
  <input type="input" placeholder="User Name">
  <input type="password" placeholder="Password">
  <p class="lostCredentials">Lost Your Credentials</p>
  <router-link to="/welcome"><div class="mx-auto d-block log-arrow"><i class="fas fa-chevron-right"></i></div></router-link>
  <router-view/>
</section>
</transition>
<section class="signIn" v-if="isShow['Sign']">
<h2 class="text-center">please sign in</h2>
<div class="mx-auto d-block sign-arrow" @click="isShow['Log'] = !isShow['Log']; isShow['Sign'] = !isShow['Sign']"><i class="fas fa-chevron-down"></i></div>
</section>
    <section class="container">
      <section class="main-illustration">
        <img alt="House" src="../assets/Img_Asset.png" class="mx-auto d-block">
      </section><!-- End Main Illustration -->
      <section class="logo">
        <img alt="logo" src="../assets/Logo_Asset.png" class="mx-auto d-block">
      </section><!-- End logo -->
      <h1 class="text-center mt-2">welcome to our online referral portal</h1>
      <Button></Button>
    </section><!-- End Container -->
  </div>
</template>

<script>
import Button from '@/components/ui/Button.vue'
export default {
  name: 'LogIn',
  components: {
    Button
  },
  data(){
  return{
    isShow:{
      'Sign': true,
      'Log': false,
    }
  }
},
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->

<style lang="scss">
@import "../styles/universal.scss";
@import "../styles/log-in.scss";
</style>
