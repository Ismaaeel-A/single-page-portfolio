<template>
  <div class="wrapper">
    <NavBar />
    <main class="container-fluid">
      <router-view />
    </main>
    <footer-comp/>
  </div>
</template>

<script>
import NavBar from './components/NavBar.vue'
import FooterComp from './components/Footer.vue'
/* import LandingVue from './components/Landing.vue' */

export default {
  components: {
    NavBar,
    FooterComp
  }
}
</script>


<style src="./assets/css/style.css"></style>
