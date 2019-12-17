<template>
  <main class="welcome">
    <Nav></Nav>
    <section class="main-illustration container">
      <img alt="House" src="../assets/Img_Asset.png" class="mx-auto d-block">
      <h1>Welcome {{name}}</h1>
      <p>Would you like to start a new lead?</p>
      <Button>New Lead</Button>
    </section><!-- End Main Illustration -->
  </main>
</template>

<script>
// @ is an alias to /src
import Button from '@/components/ui/Button.vue'
import Nav from '@/components/ui/Nav.vue'

export default {
  name: 'welcome',
  components: {
    Nav,
    Button,
  },
  data(){
  return{
    name:"Forename",
  }
},
}
</script>

<style lang="scss">
@import "../styles/lead_pages.scss";
@import "../styles/navigation.scss";
</style>
