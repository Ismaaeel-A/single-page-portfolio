<template>
  <div class="container">
    <div class="row">
      <div class="col">
        <img src="https://ismaaeel-a.github.io/allimages/Images/plc.png" alt="profile" loading="lazy">
      </div>

      <div class="col">
        <div class="details">
          <h1 class="display-1">Ismaa'eel Ahmed</h1>
          <span>{{ jobTitle[0] }}</span>
        </div>
      </div>

    </div>
  </div>
</template>

<script setup>
import { computed, onMounted } from 'vue'
const jobTitle = computed(() => this.$store.state.jobTitle)
onMounted(() => {
  this.$store.dispatch('fetchJobTitle')

})
</script>

<style></style>