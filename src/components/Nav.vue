<template>
<main id="nav-main">
  <transition name="slide">
    <section class="nav-links" v-if="showNav['Hide']">
      <ul>
        <router-link to="/"><li><i class="fas fa-unlock"></i>&nbsp; Log Out</li></router-link>
      <li><i class="fas fa-cog"></i>&nbsp; Settings</li>
        <li><i class="fas fa-user-plus"></i>&nbsp; New Lead</li>
        <li><i class="fas fa-user-friends"></i>&nbsp; Refferals</li>
        <li><i class="fas fa-user-edit"></i>&nbsp; Manage Users</li>
      </ul>
    </section>
  </transition>
  <section class="row">
    <div class="col-6">
      <img alt="logo" src="../assets/Logo_Asset.png" class="nav_logo">
    </div><!-- End col-6 -->
    <div class="col-6">
      <i class="fas fa-bars fa-2x float-right" @click="showNav['Hide'] = !showNav['Hide']; showNav['Show'] = !showNav['Show']"></i>
    </div><!-- End col-6 -->
  </section>
</main>
</template>

<script>
export default {
  name: 'navigation',
  data() {
    return {
      showNav: {
        'Show': true,
        'Hide': false,
      }
    }
  },

}
</script>
