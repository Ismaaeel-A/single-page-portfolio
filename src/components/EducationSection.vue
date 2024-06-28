<template>
  <div class="container">
    <div v-if="education?.length" class="row">
        <h3>{{ education[0]?.heading }}</h3>

        <div class="container">
            <h2>{{education[0]?.subheading1}}</h2>
            <p>{{ education[0]?.p1 }}</p>
        </div>
        <div class="container">
            <h2>{{education[1]?.subheading2}}</h2>
            <p>{{ education[1]?.p2 }}</p>
        </div>
        <div class="container">
            <h2>{{education[2]?.subheading3}}</h2>
            <p>{{ education[2]?.p3 }}</p>
        </div>
        <div class="container">
            <h2>{{education[3]?.subheading4}}</h2>
            <p>{{ education[3]?.p4 }}</p>
        </div>
    </div>
  </div>
</template>

<script setup>
import { computed, onMounted } from 'vue'
import { useStore } from 'vuex'
/* import Spinner from './Spinner.vue' */

const store = useStore()
const education = computed(() => store.state.education)

onMounted(() => {
  store.dispatch('fetchEducation')
  console.log('About Dispatch');
})



</script>





<style></style>