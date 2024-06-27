<template>
  <div class="container">
    <div class="row vh-100 align-items-center">
      <div class="col">
        <img src="https://ismaaeel-a.github.io/allimages/Images/plc.png" alt="profile" loading="lazy">
      </div>

      <div class="col">
        <div class="details">
          <h1 class="display-1">Ismaa'eel Ahmed</h1>
          <p v-if="title"><span>{{ title }}</span></p>

          <Spinner v-else/>
        </div>
      </div>

    </div>
  </div>
</template>

<script setup>
import { computed, onMounted, ref } from 'vue'
import { useStore } from 'vuex'
import Spinner from './Spinner.vue'

const store = useStore()
const jobTitle = computed(() => store.state.jobTitle)
const title = ref('rr')
const cnt = ref(-1)

function repeat() {
  try {
    if (cnt.value == jobTitle.value?.length) cnt.value = 0;
    title.value = jobTitle.value?.at(cnt.value)?.title; 
    
    setTimeout(repeat, 2000)
    cnt.value++ 
  } catch (e) {
    //
  }

}

onMounted(() => {
  store.dispatch('fetchJobTitle')
  repeat()
})

</script>

<style></style>