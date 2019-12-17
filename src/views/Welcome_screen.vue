<template>
<<<<<<< HEAD
<main class="welcome">
  <Nav></Nav>
  <section class="main-illustration container">
    <img alt="House" src="../assets/Img_Asset.png" class="mx-auto d-block">
    <h1>Welcome {{name}}</h1>
    <p>Would you like to start a new lead?</p>
    <Button>New Lead</Button>
  </section><!-- End Main Illustration -->
</main>
=======
  <main class="welcome">
    <section class="main-illustration">
      <img alt="House" src="../assets/Img_Asset.png" class="mx-auto d-block">
    </section><!-- End Main Illustration -->
  </main>
>>>>>>> parent of d477bf43... welcome screen
</template>

<script>
// @ is an alias to /src
<<<<<<< HEAD
import Button from '@/components/ui/Button.vue'
import Nav from '@/components/Nav.vue'
=======

>>>>>>> parent of d477bf43... welcome screen

export default {
  name: 'welcome',
  components: {
<<<<<<< HEAD
    Nav,
    Button,
  },
  data() {
    return {
      name: "Forename",
    }
  },
=======

  }
>>>>>>> parent of d477bf43... welcome screen
}
</script>
