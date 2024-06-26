<template>
  <div>
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

export default {
  components: {
    NavBar,
    FooterComp
  }
}
</script>


<style src="./assets/css/style.css"></style>
