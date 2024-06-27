<template>
  <div class="container">
    <div v-if="about?.length" class="row">
      <h3>{{ about[0]?.heading }}</h3>
      <p>{{ about[0]?.p1 }}</p>
      <ul>
        <li>{{ about[0]?.listItem1 }}</li>
        <li>{{ about[0]?.listItem2 }}</li>
        <li>{{ about[0]?.listItem3 }}</li>
        <li>{{ about[0]?.listItem4 }}</li>
      </ul>

      <p>{{ about[0]?.p2 }}</p>
    </div>
  </div>
</template>

<script setup>
import { computed, onMounted } from 'vue'
import { useStore } from 'vuex'
/* import Spinner from './Spinner.vue' */

const store = useStore()
const about = computed(() => store.state.about)
/* const heading = about.value.heading */
/* console.log(about); */

onMounted(() => {
  store.dispatch('fetchAbout')
  console.log('About Dispatch');
})
</script>

<style></style>